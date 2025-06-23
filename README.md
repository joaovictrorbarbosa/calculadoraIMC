Aqui neste projeto, foi criado uma simples calculadora de IMC.

O calculo do IMC (Índice de Massa Corporal), é uma ferramenta para avaliar o peso de uma pessoa em relação à sua altura e é usada para classificar o estado nutricional. Os resultados são divididos em categorias como abaixo do peso, normal, sobrepeso e obesidade, com diferentes graus de obesidade. 

Para o projeto, utilizei a IDE SublimeText, linguagem Java, e a plataforma de criação de interfaces JavaFX.

## 📸 Interface

A interface é composta por:
- Campos de entrada para peso e altura
- Um botão para realizar o cálculo
- Um label que exibe o resultado do IMC

## 🧮 Fórmula utilizada para calculo

IMC = Peso / altura²

- Peso e altura foram transformados de String, em double, para que o calculo seja preciso, da seguinte forma:
- double peso = Double.parseDouble(campoPeso.getText().replace(',', '.'));
- double altura = Double.parseDouble(campoAltura.getText().replace(',', '.'));

double imc = peso / (altura * altura);

## 🚀 Como executar

1. Certifique-se de ter o **Java JDK 8+** e o **JavaFX configurado** no seu ambiente.
2. Clone este repositório:

```bash
git clone https://github.com/seu-usuario/ProjetoIMC.git
```

## 📄 Exemplo de uso

1. Insira seu **peso em kg** (por exemplo, `70`)
2. Insira sua **altura em metros** (por exemplo, `1.75`)
3. Clique em **"Calcular IMC"**
4. O resultado será exibido no formato: Seu IMC é: 22.86


## ⚠️ Observações

- O aplicativo lida com **vírgulas e pontos como separadores decimais** (`1,75` ou `1.75`)
- Se valores inválidos forem inseridos, uma **mensagem de erro será exibida**

