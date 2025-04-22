<template>
  <div>
    <h1>Calculadora Aritmética</h1>
    <div>
      <input type="number" v-model="number1" placeholder="Número 1" />
      <input type="number" v-model="number2" placeholder="Número 2" />
      <select v-model="operation" @change="calculate">
        <option value="+">Adicionar</option>
        <option value="-">Subtrair</option>
        <option value="*">Multiplicar</option>
        <option value="/">Dividir</option>
      </select>
    </div>
    <h2>Resultado: {{ result }}</h2>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number1: 0,
      number2: 0,
      operation: '+',
      result: 0,
    };
  },
  watch: {
    number1: 'calculate',
    number2: 'calculate',
    operation: 'calculate',
  },
  methods: {
    calculate() {
      const num1 = parseFloat(this.number1);
      const num2 = parseFloat(this.number2);
      switch (this.operation) {
        case '+':
          this.result = num1 + num2;
          break;
        case '-':
          this.result = num1 - num2;
          break;
        case '*':
          this.result = num1 * num2;
          break;
        case '/':
          this.result = num2 !== 0 ? num1 / num2 : 'Erro: Divisão por zero';
          break;
        default:
          this.result = 0;
      }
    },
  },
};
</script>

<style scoped>
h1 {
  font-size: 2em;
}
input {
  margin: 0.5em;
}
</style>