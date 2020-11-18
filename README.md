Tarefas:

1. Estender `Account` com a interface `BusinessAccount`. Acrescentar os métodos:

        double getLoanLimit();
        void setLoanLimit(double loanLimit);
        void loan(double amount, double operationCost) throws InvalidAmountException;
    
    O método `loan` levanta a exceção quando o valor a pedir emprestado excede o
    limite de crédito.
   
2. Implementar `BusinessAccount` com uma classe `BusinessAccountClass`, que oferece os mesmos métodos que `AccountClass`, além dos métodos de `BusinessAccount`.

3. Criar a interface `InterestRateInstrument` para representar um instrumento sujeito a uma taxa de juro.
   
        void setRate(double rate) throws NegativeRateException;
        double getRate(double rate);
        void updateBalance();
    
    O método `setRate` levanta uma exceção quando o valor da taxa de juro é
    negativo.
    
4. Criar uma classe `SavingsAccount`, que estende `AccountClass` e implementa
   `InterestRateInstrument`
   
5. Implementar testes unitários para as classes desenvolvidas.
