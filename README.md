<h1 align="center">NLW#4 - Moveit - aula 01</h1> 

<img src=".github/Wallpaper.png">


### :mag: Sobre o projeto 
Esta aplicação juntou o mundo dos games com a parte de ganhar xp e subir de nível com a técnica do pomodoro. Pomodoro pra quem não conhece é um contador de tempo de 25 minutos onde você mantém o foco no estudo ou trabalho, e após tem 5 minutos de descando pra fazer qualquer outra atividade. Nesta aplicação os intervalos são marcados por tarefas que, se cumpridas, dão xp pra você subir de nível. As tarefas consistem em atividades como caminhar por 3 minutos para que pessoas que usam muito o computador no seu dia a dia não sofram com problemas futuros de ficar muito tempo sem se movimentar.

### 💻 Nesta aula

* Fluxo de uma API Rest ou Restful: Qualquer dispositivo seja mobile, desktop, tv fazem uma requisição ao backend que retorna um JSON, e o frontend do dispositivo por sua vez é  responsável por interpretar e renderizar pelo dispositivo que o chamou de sua forma particular. Diferente de aplicações em modelo antigo onde deveriam ser criadas rotas separadas para cada tipo de dispositivo, gerando maiores problemas para manutenção por exemplo e sobrecarregando o backend da aplicação.
* React: O react entra no fluxo da api na parte do browser, ou seja, o frontend. Com este framework a aplicação se torna muito mais performática já que nela ficam os códigos html, css e javascript sem que precise ser retornado do servidor. É uma biblioteca de construção de interfaces muito fluída e reativa a interação do usuário sem precisar recarregar a interface por completo.
* Typescript: Basicamente o javascript com tipagem estática. Maior controle de tipos de dados, criação de tipos personalizados, deixa o desenvolvimento mais inteligente por mostrar o que contém este tipo de dado ou ao chamar uma função saber exatamente o tipo de dado que é requisitado diminuindo chances de erros.
* create-react-app: Uma forma simplificada de criar um projeto em react onde é montada a estrutura com babel, webpack, node de forma automática.
* Componentes: código react é feito basicamente com componentes, ou seja, se tenho um botão que se repete em minha aplicação ele pode ser um componente, um cabeçalho pode ser um componente. Seriam pequenos trechos de códigos que se retirados do contexto, o restate da aplicação ainda faz sentido e podem ser usados diversas vezes em diferentes locais ou na mesma página.
* Propriedades: Forma de passar informações para cada componente. Para recuperar as informações, todos os componentes recebem props e nelas contém como se fosse um objeto para acessar essas propriedades(código abaixo). Também existe as propriedades do tipo children, que são passadas dentro do componente(código abaixo).
```
<Button color="red">
    Botão 1
</Button>

interface ButtonProps {
  color:string;
  children: string;
}

export function Button(props:ButtonProps){
  return (
    <button type="button" style={{backgoundColor: props.color}}>
      {props.color} {props.children}
    </button>
  )
}
```
* Estado: Armazena informação dentro do componente, ou seja, o estado dele que vai mudar ao longo do tempo. Por exemplo no click de um botão aumentar em 1 o seu valor. Este valor deve ser armazenado em um estado. O método useState retorna uma variável e uma função que cria uma novo estado a partir do estado anterior sem modificar, respeitando a imutabilidade.

```
const [counter, setCounter] = useState(1);

```
* *.module.css: criação de estilo personalizado para cada componente ou página de forma a não afetar outros componentes na aplicação.

Além destes conceitos foram criados os estilos globais da aplicação, o primeiro componente barra de experiência do usuário que foi trabalhado como header, os conceitos de font-size para acessibilidade e responsividade da aplicação.

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- [React](https://pt-br.reactjs.org/)
- HTML;
- CSS;
