<div align="center">

🧮 Calculadora de IMC
Um aplicativo Android simples e intuitivo para calcular o Índice de Massa Corporal.

Desenvolvido em Kotlin com Jetpack Compose para a disciplina de Laboratório de Programação para Dispositivos Móveis (LPDM).
</div>

📱 Sobre o projeto
A Calculadora de IMC é um aplicativo Android nativo que calcula o Índice de Massa Corporal (IMC) a partir do peso e da altura informados pelo usuário. Após tocar em Calcular, o aplicativo apresenta o valor obtido e a classificação correspondente.

O projeto foi desenvolvido como atividade prática da 2ª Avaliação de LPDM, com foco em interatividade, gerenciamento de estado e construção de interfaces com Jetpack Compose.
✨ Funcionalidades
- ⚖️ Informar o peso em quilogramas, incluindo valores decimais.
- 📏 Informar a altura em metros, incluindo valores decimais.
- 🧮 Calcular o IMC por meio do botão Calcular.
- 🔢 Ativar ou desativar a opção Arredondar resultado.
- 📊 Visualizar o valor calculado e a classificação correspondente.
📐 Fórmula do IMC
O cálculo utilizado é:
IMC = peso (kg) / (altura (m) × altura (m))
Exemplo: para uma pessoa com 70 kg e 1,75 m:
IMC = 70 / (1,75 × 1,75)
IMC ≈ 22,86
Classificação utilizada
IMC	Classificação
Menor que 18,5	Abaixo do peso
De 18,5 até 24,9	Peso normal
De 25,0 até 29,9	Sobrepeso
30,0 ou mais	Obesidade


Este aplicativo tem finalidade acadêmica e informativa; o resultado do IMC, isoladamente, não substitui uma avaliação profissional de saúde.

🛠️ Tecnologias
- Kotlin — linguagem de programação.
- Jetpack Compose — criação da interface de usuário declarativa.
- Android Studio — ambiente de desenvolvimento.
- Gradle — compilação e gerenciamento das dependências.
- Git e GitHub — versionamento e hospedagem do código.
Ambiente de desenvolvimento: preencha aqui a versão do Android Studio utilizada no projeto.

🚀 Como executar
Pré-requisitos
- Android Studio instalado.
- Android SDK compatível com as configurações do projeto.
- Emulador Android configurado ou dispositivo físico com depuração USB habilitada.
Executando pelo Android Studio
1. Clone este repositório:
   git clone <URL_DO_REPOSITORIO>
2. Abra a pasta kotlin-calculadora-imc no Android Studio.
3. Aguarde a sincronização do Gradle.
4. Inicie um emulador pelo Device Manager ou conecte um dispositivo Android.
5. Selecione a configuração de execução do aplicativo.
6. Clique em Run ▶ para compilar e executar.
7. Informe o peso e a altura, escolha se deseja arredondar o resultado e pressione Calcular.
🧩 Organização do código
Ajuste os nomes desta seção para corresponder exatamente aos arquivos e às funções presentes no repositório.
Arquivo ou função	Responsabilidade
MainActivity.kt	Ponto de entrada da aplicação e configuração do conteúdo da interface.
CalculadoraIMC	Composable responsável por organizar os elementos da tela principal.
EditNumberField	Campo de texto reutilizável para entrada de valores numéricos, com value e onValueChange.
calcularIMC	Função responsável pelo cálculo do Índice de Massa Corporal, separada da interface.
Função de classificação	Determina a categoria do IMC com uma expressão when.
object de constantes	Centraliza os limites das faixas de classificação.
ui/theme/	Arquivos de tema visual, caso presentes no projeto.
AndroidManifest.xml	Contém declarações e configurações essenciais da aplicação Android.


🌳 Hierarquia da interface
Exemplo ilustrativo; adapte os nomes conforme a implementação:
MainActivity
└── CalculadoraIMC
    ├── Título
    ├── EditNumberField (peso)
    ├── EditNumberField (altura)
    ├── Switch (arredondar resultado)
    ├── Button (Calcular)
    └── Resultado
        ├── Valor do IMC
        └── Classificação
🧠 Conceitos praticados
- Jetpack Compose: construção de interface sem layouts XML.
- Gerenciamento de estado: uso de remember e mutableStateOf para atualizar a tela.
- State hoisting: passagem de estado e callbacks para componentes reutilizáveis.
- Conversão segura de valores: uso de toDoubleOrNull() e do operador ?:, evitando o operador !!.
- Separação de responsabilidades: lógica de cálculo independente da interface.
- Expressão when: seleção da classificação de acordo com as faixas de IMC.
- Organização de constantes: centralização dos limites para evitar números mágicos.
👨‍💻 Autor
- Aluno: [Seu nome completo]
- Turma: [Sua turma]
- Disciplina: Laboratório de Programação para Dispositivos Móveis (LPDM)
- Professor: MSc Rodrigo de Lima Cunha
<div align="center">

Feito como projeto acadêmico para a 2ª Avaliação prática de LPDM.
</div>
