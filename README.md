
## Carousel com Animação e Interatividade

### Descrição
Este projeto implementa um carousel totalmente funcional, construído com HTML, CSS e JavaScript. O carousel exibe uma coleção de imagens com sobreposições de texto descritivo e botões de navegação. Os usuários podem navegar pelas imagens utilizando as setas "Anterior" e "Próximo". O carousel conta com transições suaves e animações que melhoram a experiência do usuário.

## Principais Características:
Slider Automático de Imagens: O carousel desliza automaticamente após um intervalo definido.
Navegação Manual: Os usuários podem navegar pelas imagens clicando nas setas "Próximo" e "Anterior".
Pré-visualização de Miniaturas: Miniaturas das imagens são exibidas na parte inferior, permitindo que os usuários vejam uma prévia do conteúdo.
Design Responsivo: O layout se adapta a telas menores (por exemplo, dispositivos móveis).
Animações de Conteúdo: Várias animações são aplicadas ao conteúdo e às imagens, incluindo efeitos de deslizamento e transições de opacidade.

## Estrutura de Arquivos
HTML: Estrutura da página, incluindo o carousel, navegação e conteúdo das imagens.
CSS: Estilo do carousel e da página, incluindo animações.
JavaScript: Implementa a funcionalidade de navegação, deslizar automaticamente e alternar imagens.
Como Funciona
HTML:
A estrutura HTML define um contêiner carousel com vários itens, cada um contendo uma imagem e conteúdo sobreposto (por exemplo, título, descrição, botões). O carousel possui dois componentes principais:

Lista do Carousel: Contém os itens principais (imagens com conteúdo).
Seção de Miniaturas: Exibe versões menores das imagens como pré-visualizações clicáveis.
Setas de Navegação: Botões que permitem ao usuário navegar para a próxima ou anterior imagem.
CSS:
O CSS gerencia a aparência geral do carousel:

Posicionamento: As imagens são configuradas para cobrir toda a largura e altura da tela, com o conteúdo centralizado sobre as imagens.
Animações de Texto: Cada elemento de conteúdo (por exemplo, título, descrição, botões) possui um efeito de animação (por exemplo, fade-in e deslizar para cima).
Estilos de Miniaturas: As miniaturas são posicionadas na parte inferior e animam em resposta ao estado do carousel (próximo ou anterior).
JavaScript:
O JavaScript controla o comportamento interativo do carousel:

Navegação: Funções são ativadas quando o usuário clica nas setas "Próximo" ou "Anterior".
Deslizamento Automático: O carousel move-se automaticamente para a próxima imagem após um intervalo definido (timeAutoNext).
Conteúdo Dinâmico: Quando o carousel se move, o conteúdo e as imagens deslizam para dentro e para fora com animação, garantindo transições suaves.
Controle de Tempo: Uma barra de tempo (time) mostra o tempo restante para a imagem atual antes de mudar automaticamente.
Animações e Efeitos
Animação de Conteúdo:
Para o primeiro item do carousel, o conteúdo (autor, título, tópico, descrição e botões) começa fora da tela e embaçado. Ao longo de 1,8 segundos, o conteúdo desliza para o seu lugar com total opacidade:

showContent: Animação de keyframe usada para fazer o conteúdo aparecer com desfoque e deslocamento.
Transições de Imagem:
Ao navegar para a próxima ou anterior imagem:

Animação "Próxima": A imagem da nova tela aparece animando de um tamanho pequeno (miniatura) para o tamanho total. A animação showImage realiza esse efeito.
Animação "Anterior": Ao voltar, a imagem move-se de um tamanho grande de volta para uma miniatura menor, utilizando a animação outFrame.
Animações de Miniaturas:
As miniaturas se movem para dentro e para fora da tela quando a imagem muda:

showThumbnail: As miniaturas aparecem suavemente quando entram na tela.
effectNext: As miniaturas se movem horizontalmente quando a próxima imagem é ativa.
Timer de Execução:
Uma barra de tempo animada no topo do carousel indica quanto tempo cada imagem ficará visível antes de ser automaticamente substituída pela próxima. Isso é gerido pela animação de keyframe runningTime.

## Como Usar
Botões "Próximo"/"Anterior": Clique nos botões de seta (< e >) para navegar manualmente pelo carousel.
Deslizamento Automático: O carousel mudará automaticamente para a próxima imagem após 7 segundos (timeAutoNext).
Miniaturas: Você também pode interagir com as miniaturas menores na parte inferior do carousel para visualizar imagens específicas.
Responsivo: O carousel se adapta a diferentes tamanhos de tela, proporcionando uma experiência sem interrupções em dispositivos móveis e desktop.
Personalização
Imagens: Substitua as fontes das imagens no HTML com seus próprios arquivos de imagem.
Texto: Modifique o conteúdo dentro dos elementos .content para atualizar os títulos, descrições e outros textos sobrepostos.
Velocidade e Tempo: Ajuste a variável timeAutoNext para mudar o intervalo entre cada slide, ou modifique o runningTime para controlar a velocidade da barra de tempo.
Dependências
Fonte: A fonte usada neste carousel é Poppins, carregada do Google Fonts.
Navegador Moderno: Este carousel depende de animações CSS e JavaScript, sendo ideal para navegadores modernos que oferecem suporte completo a essas tecnologias.

## Conclusão
Este carousel oferece uma experiência de deslizar suave e visualmente atraente, com elementos interativos e animações. É um excelente exemplo de como combinar HTML, CSS e JavaScript para criar uma interface dinâmica e amigável para exibir galerias de imagens ou slideshows.
