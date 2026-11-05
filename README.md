# Vai Chover na Próxima Hora? — simulador de decisão

Pequeno projecto de aprendizagem em HTML, CSS e JavaScript. Apresenta um contador regressivo e uma decisão aleatória entre **SIM** e **NÃO**.

> **Importante:** apesar do título, esta versão **não faz uma previsão meteorológica**. Não consulta serviços de meteorologia, não pede a localização do utilizador e não analisa dados climáticos. A resposta é simulada por um sorteio aleatório no código.

## Sobre o projecto

A página demonstra uma interface simples com contagem decrescente, actualização visual da decisão e uma animação discreta quando o resultado muda. A decisão **SIM** tem uma probabilidade aproximada de 45% na lógica actual; **NÃO** é o resultado nos restantes casos.

Este exercício integra o percurso contínuo de aprendizagem e desenvolvimento de competências de **Benjamim Tanislau José Cacuengue**.

## Funcionalidades implementadas

- Contador regressivo com duração inicial de 60 minutos.
- Sorteio de uma decisão entre **SIM** e **NÃO**, usando JavaScript nativo.
- Intervalo nominal de 10 minutos entre decisões durante o ciclo.
- Apresentação visual dos resultados e animação quando o texto da decisão muda.
- Folha de estilos com uma regra de adaptação para ecrãs estreitos.

Os sorteios nos limites inicial e final do temporizador podem ocorrer mais vezes do que o intervalo nominal sugere. O contador também reinicia quando a página é recarregada; não guarda o progresso.

## Tecnologias

- HTML5
- CSS3
- JavaScript nativo (Vanilla JavaScript)
- APIs do navegador: DOM, `setInterval`, `MutationObserver` e Web Animations API

O projecto não declara dependências externas, ferramentas de compilação ou um processo de instalação.

## Como consultar

1. Obter uma cópia do repositório:

   ```bash
   git clone https://github.com/tanislaucacuengue/contador.git
   cd contador
   ```

2. Abrir `index.html` num navegador Web actualizado.

Não é necessário instalar pacotes nem executar um comando de compilação para consultar esta página estática. Não existe um servidor de desenvolvimento definido pelo projecto.

## Estrutura dos ficheiros

| Ficheiro | Função |
| --- | --- |
| [`index.html`](index.html) | Estrutura da página e conteúdo inicial. |
| [`style.css`](style.css) | Apresentação visual e adaptação a ecrãs estreitos. |
| [`script.js`](script.js) | Contagem regressiva, sorteio das decisões e animação. |

## Limitações desta versão

- A aplicação **não prevê chuva** nem representa dados meteorológicos reais; não deve ser usada para decisões relacionadas com o tempo.
- A resposta é aleatória e não está associada a uma cidade, localização ou fonte meteorológica.
- O temporizador baseia-se em actualizações periódicas do navegador; o seu ritmo pode variar se a página ficar em segundo plano.
- A lógica actual pode gerar sorteios adicionais no início e no fim do ciclo. A indicação de uma próxima decisão nesses momentos não significa que exista uma previsão ou um novo ciclo activo.
- A página ainda pode beneficiar de melhorias de acessibilidade, incluindo a revisão do papel ARIA e do contraste do título.
- Não foram encontrados ficheiros de testes automatizados nem um ficheiro de licença nesta versão do repositório.

## Possíveis evoluções

Como trabalho futuro, o projecto poderá corrigir os limites do temporizador, reforçar a acessibilidade e, se esse for o objectivo, integrar uma fonte meteorológica real com atribuição adequada. Até essa integração ser efectivamente implementada e validada, a aplicação deve continuar identificada como uma simulação.

---

**Desenvolvimento:** Benjamim Tanislau José Cacuengue.

Este projecto faz parte do meu percurso de aprendizagem: cada exercício é uma oportunidade para praticar, rever decisões técnicas e continuar a desenvolver competências em programação Web.
