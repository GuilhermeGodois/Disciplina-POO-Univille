# Trabs


Questionário Introdução Orientação Objeto

1. É uma coisa, entidade, qualquer coisa que possa imaginar
e que tenha uma identidade.

2. Caracteristicas Carro = Cor, Modelo, Marca
   Comportamentos  Carro = Anda, Para, Abre a porta
   
3. Caracteristicas são consideradas atributos e Comportamentos são considerados métodos

4. O POO tem por objetivo desenvolver software utilizando objetos de maneira cooperativa através de troca de mensagens

5. A abstração na POO consiste em trabalhar um objeto dentro da programação se preocupando somente com suas principais propriedades,
sem se apegar a pontos acidentais
exemplo: Carros > modelos

6. Encapsula características em comum de um grupo de objetos. Define os atributos e métodos que o objeto poderá possuir.

7. Camelcase. Exemplo: CalculaDesconto()

8. Alternativa Certa 4. CarroEletrico

9. Camelcase. Exemplo: corExterna

10. Alternativa Certa 3. corDeFundo

11. Camelcase. Exemplo: corExterna

12. Alternativa Certa 1.estaVazio

13. É uma coisa, entidade, qualquer coisa que possa imaginar e que tenha uma identidade.
    Ele sxiste no momento que ele é instanciado na memória
    Ele deixa de existir no momento em que ele é encerrado    

14. Quando há a criação de um novo objeto

15. È um metodo especial ou operador especial utilizado para iniciar objetos
    É ser utilizado para iniciar variáveis, instanciar outros objetos necessários, disparar métodos de inicialização.
    O construtor deve possuir o mesmo nome da Classe
    Classe NomeCarro construtor NomeCarro   

16. O próprio compilador o cria

17. Aluno p = new Aluno();

18. Trata-se de um mecanismo que possibilita restringir o acesso a variáveis e métodos da classe (ou até a própria classe).

19. Permitir a todos acessarem um determinado atributo ou método

20. Os membros da classe definidos como não podem ser acessados ou usados por nenhuma outra classe.
    Impedir que ninguém consiga nodificar ou ler o atributo em questão

21. É através dos modificadores de acesso
public class Aluno{ 
   private String matricula;
}

22. Obter informações. Esse tipo de método sempre retorna um valor
Exemplo: TextField trazNome = new TextField();
         traznome.setText(nome.getText());

23. Definir valores. Esse tipo de método geralmente não retorna valores
Exemplo: TextField nome = new TextField();
         nome.setText("FULANO");
         
24. O Nome da Clase; Os Atributos e os Métodos

25. Camelcase com a primeira letra minuscula 

26. Camelcase com a primeira letra minuscula 

27. 

28.
(-) refere-se a um atributo ou método que pode ser usado
somente na classe onde foi criado;
(+) refere-se a um atributo ou método que pode ser usado
por qualquer classe do diagrama, ou seja, são atributos ou métodos públicos;
(#)  refere-se  a  um  atributo  ou  método  que  pode  ser  usado
somente  pela  classe onde foi criado e também pelas classes derivadas desta.

29.
| Cliente                                                                     |
|-----------------------------------------------------------------------------|
| -nome: String <br/>-email: String <br/>-telefone:String                     |
| +setNome(nome: String) <br/>+setEmail(email: String) <br/>+setTelefone(telefone: String) <br/>+getNome(): String <br/>+getEmail(): String <br/>+getTelefone(): String |

30.
```java
public class Cliente {
        
    private String nome;
    private String email;
    private String telefone;
        
    public void Cliente(String iNome, String iEmail, String iTelefone) {
        this.nome = iNome;
        this.email = iEmail;
        this.telefone = iTelefone;
    }
       
    public void setNome(String novoNome) {
        this.nome = novoNome;
    }
        
    public void setEmail(String novoEmail) {
        this.email = novoEmail;
    }
        
    public void setTelefone(String novoTelefone) {
        this.telefone = novoTelefone;
    }
        
    public String getNome() {
        return nome;
    }
    
    public String getEmail() {
        return email;
    }
    
    public String getTelefone() {
        return telefone;
    }
        
}
```

31.
Produto:
```java
public class Produto {
        
    private String nome;
        
    public Produto(String iNome) {
        this.nome = iNome;
    }
       
    public void setNome(String novoNome) {
        this.nome = novoNome;
    }
    
    public String getNome() {
        return nome;
    }
}
```
Password:
```java
public class Password {
        
    private String value;
        
    public void Password(String iValue) {
        this.value = iValue;
    }
       
    public boolean isEqual(String eValue) {
        return (value == eValue);
    }
}
```
Animal:
```java
public class Password {
        
    private boolean alive;
        
    public boolean isAlive() {
        return alive;
    }
       
    public boolean die() {
        this.alive = false;
    }
}
```
32.
| Livro                                                                       |
|-----------------------------------------------------------------------------|
| -nome: String                     |
| +setNome(nome: String) <br/>+getNome(): String |

| ContaCorrente                                                               |
|-----------------------------------------------------------------------------|
| -saldo: double                     |
| +sacar(valor: double): double <br/>+depositar(double valor) <br/>-recalcularSaldo() |

| Par                                                               |
|-----------------------------------------------------------------------------|
| +chave: string <br/>+valor: string                     |
| <br/> |

| Impressora                                                               |
|-----------------------------------------------------------------------------|
| <br/> |
| +imprimir(Documento documento) |

