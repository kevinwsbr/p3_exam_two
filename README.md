
# Prova II - Projeto de software

## Descrição do projeto
O objetivo do projeto é construir um sistema de folha de pagamento. O sistema consiste de um banco de dados de empregados de uma empresa além dos seus dados associados tais como cartões de ponto. O sistema deve pagar cada empregado. Empregados devem receber o salário correto, no momento correto, usando o método que eles preferem. Além do mais, várias taxas e impostos são deduzidos do seu salário [\[...\]](https://docs.google.com/viewer?a=v&pid=sites&srcid=aWMudWZhbC5icnxjb21wMjE1fGd4OjFjYWZlZTlkYTYwZmJjOWQ)

## Diagrama de classes
Uma possível implementação para esse projeto foi modelada da seguinte forma:

![enter image description here](https://raw.githubusercontent.com/kevinwsbr/p3_exam_two/master/Diagrama%20de%20classe%20UML.png)

## Padrões utilizados
### Singleton
Na classe `System` houve a implementação do padrão Singleton com o objetivo de garantir que apenas haja uma única instância deste objeto disponível - por meio do método `getInstance()`.

### Memento
O padrão Memento foi implementado na classe `System` com o propósito de salvar os estados do sistema (empregados, agendas, pontos, etc) a cada alteração. O objeto `Caretaker` é responsável por fazer a gerência do objeto `SystemMemento` que, por sua vez, implementa a interface `Memento` e efetivamente guarda as cópias dos estados do sistema nas transações em que se faz necessário o uso de undo/redo.

## Demais classes
As demais classes foram criadas de acordo com os requisitos funcionais solicitados na descrição do projeto.
