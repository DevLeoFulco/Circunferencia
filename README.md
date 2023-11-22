**README - Métodos Estáticos no Código de Circunferencia**

Este projeto Java consiste em dois arquivos: `Program.java` e `Calculadora.java`. Vamos focar na compreensão dos métodos estáticos e como eles estão sendo aplicados no código.

### Métodos Estáticos:

1. **O que são Métodos Estáticos?**

   Métodos estáticos são membros de uma classe que pertencem à própria classe, em vez de instâncias específicas dessa classe. Eles podem ser chamados diretamente na classe, sem a necessidade de criar uma instância dessa classe.

2. **Utilização de Métodos Estáticos no Código:**

   - **`Calculadora.java`:**
  
      - **`public static final double PI`**: Aqui, temos uma variável constante (final) chamada `PI` que armazena o valor de π (pi). Por ser `static`, ela pertence à classe `Calculadora` e pode ser acessada diretamente sem criar uma instância da classe.

      - **`public static double circunferencia(double raio)`**: Este método calcula a circunferência com base no raio fornecido. Novamente, é estático, o que significa que pode ser chamado diretamente na classe `Calculadora`.

      - **`public static double volume(double raio)`**: Similar ao método `circunferencia`, este método calcula o volume de uma esfera com base no raio. Ele também é estático.

   - **`Program.java`:**

      - **`public static void main(String[] args)`**: O método principal `main` é o ponto de entrada do programa. Note que é estático. Dentro deste método, são chamados métodos estáticos da classe `Calculadora` diretamente, sem a necessidade de criar uma instância.

3. **Como os Métodos Estáticos Estão Sendo Utilizados:**

   - No método `main` em `Program.java`, os métodos `Calculadora.circunferencia(raio)` e `Calculadora.volume(raio)` são chamados diretamente, sem a criação de um objeto da classe `Calculadora`. Isso é possível porque ambos os métodos na classe `Calculadora` são estáticos.

   - A variável `Calculadora.PI` também é acessada diretamente na classe `Program`, sem a necessidade de criar uma instância da classe `Calculadora`, pois é uma variável estática.

4. **Vantagens dos Métodos Estáticos:**

   - **Simplicidade:** A principal vantagem é a simplicidade. Você pode chamar métodos estáticos sem criar instâncias da classe, tornando o código mais direto.

   - **Acesso Universal:** Métodos estáticos podem ser acessados de qualquer lugar do código sem a necessidade de instanciar a classe. Isso é útil para funcionalidades que não dependem do estado de instância.

**Conclusão:**

O uso de métodos estáticos neste código simplifica a chamada de funcionalidades da classe `Calculadora`, tornando o código mais limpo e direto. A compreensão dos conceitos de métodos estáticos é crucial para a construção de código Java eficiente e modular.
