# Especificação funcional — Axé Cria

## 1. Visão do projeto

**Nome:** Axé Cria, com a iniciativa atual Axé Criativo  
**Tipo:** website institucional, cultural, de agendamentos e divulgação/venda de livro  
**Formato:** página única com navegação por âncoras e rolagem suave  
**Idioma inicial:** português brasileiro (`pt-BR`)

Axé Cria é uma produtora cultural de terreiro voltada à cultura e ao empreendedorismo de terreiro. Foi fundada no Ilê Obá Axé Ogum Onirê, em Pernambuco, pelo Babalorixá Jorge Roseno de Ogum. A iniciativa realiza atividades gratuitas e abertas aos povos de terreiro com apoio do Centro de Educação e Cultura Daruê Malungo.

O website deve apresentar a iniciativa e sua história, dar visibilidade às atividades realizadas, facilitar o contato e o agendamento de atendimentos e apresentar o livro *Raízes do Corpo* para compra ou pedido.

## 2. Objetivos e público

### Objetivos

- Apresentar a identidade, a história, a missão e as pessoas por trás da Axé Cria.
- Divulgar registros de atividades culturais e permitir que visitantes encontrem atividades por categoria.
- Direcionar visitantes interessados em consultas para agendamento via WhatsApp.
- Apresentar o livro *Raízes do Corpo* e encaminhar o visitante ao canal de compra ou pedido definido pelo projeto.
- Dar crédito visível aos apoiadores e às instituições responsáveis pelo financiamento público.

### Público principal

- Povos de terreiro e pessoas interessadas em cultura, saberes e empreendedorismo de terreiro.
- Pessoas interessadas em participar das atividades, agendar atendimentos ou adquirir o livro.
- Parceiros, apoiadores, agentes culturais e instituições públicas.

## 3. Identidade visual e experiência

### Paleta oficial

| Uso | Cor | HEX |
| --- | --- | --- |
| Azul fechado — cor principal; títulos, navegação, botões primários e rodapé | RGB 0, 35, 147 | `#002393` |
| Azul claro — acentos, destaques, links e botões secundários | RGB 69, 176, 222 | `#45B0DE` |
| Verde escuro — fundos alternativos e elementos de apoio | RGB 29, 86, 53 | `#1D5635` |
| Verde vivo — chamadas de ação e agendamentos | RGB 0, 132, 53 | `#008435` |
| Fundo — off-white claro com textura sutil de papel artesanal/reciclado | A definir | A definir |

Usar textura e marcas d'água com baixa intensidade, sem reduzir contraste ou legibilidade. A textura deve ser decorativa e não competir com fotografias, texto ou controles.

### Tipografia e componentes

- Usar Alekan Rounded em suas variações Regular, Semibold, Bold e Extrabold. Confirmar disponibilidade dos arquivos e respectivas licenças antes da publicação; prever uma fonte substituta arredondada caso a fonte não carregue.
- Usar cantos arredondados de 12 a 16 px nos componentes, conforme o guia visual.
- Manter hierarquia tipográfica clara, boa legibilidade e contraste adequado entre texto e fundo.
- Aplicar estados perceptíveis de foco, hover, pressionado, selecionado e desabilitado aos controles interativos.

## 4. Estrutura da página

A página terá, nesta ordem, cabeçalho fixo, apresentação (hero), Quem Somos, Atividades Realizadas, Atendimentos & Consultas, Loja / Livro Raízes do Corpo e rodapé. O menu direciona para as seções por âncoras na própria página.

### 4.1 Cabeçalho fixo

**Conteúdo:**

- Assinatura horizontal da marca: “Axé Cria” e o slogan “Empreendedorismo, cultura e as raízes do corpo ancestral”.
- Links: Quem Somos, Atividades, Atendimentos, Livro e Contato.
- Link para o Instagram `@axe.cria`, com ícone e nome acessível.

**Comportamento:**

- Permanecer disponível durante a rolagem sem encobrir o título da seção ao navegar por âncora.
- Cada link rola até sua seção correspondente e atualiza o estado ativo do menu quando aplicável.
- Em telas estreitas, substituir os links por um botão de menu acessível. Abrir/fechar o menu por toque, teclado e leitor de tela; fechar após selecionar um destino.
- O botão do menu informa seu estado expandido/recolhido e mantém foco visível.

### 4.2 Apresentação (hero)

**Conteúdo:**

- Assinatura circular da marca.
- Título: **“Axé Cria: Produtora Cultural de Terreiro”**.
- Subtítulo apresentando a iniciativa no Ilê Obá Axé Ogum Onirê, em Pernambuco, e sua atuação cultural.
- Navegação pelas seções pelo menu do cabeçalho e pelo indicador de rolagem ao fim do hero, que leva à galeria de atividades.
- O agendamento via WhatsApp fica exclusivamente na seção **Atendimentos & Consultas**, nos cards dos profissionais.

Os textos descritivos finais e as imagens oficiais devem ser fornecidos ou aprovados pelo projeto. Não substituir as assinaturas oficiais por texto estilizado quando os arquivos de marca estiverem disponíveis.

### 4.3 Quem Somos

Apresentar, em texto e imagens aprovados pelo projeto:

- A história do Ilê Obá Axé Ogum Onirê e sua relação com a produtora.
- A missão da Axé Cria e sua atuação em cultura e empreendedorismo de terreiro.
- O perfil do idealizador, Babalorixá Jorge Roseno de Ogum.
- O apoio do Centro de Educação e Cultura Daruê Malungo.

Organizar o texto em blocos curtos, com títulos e imagens legendadas quando houver contexto relevante. Não criar fatos biográficos, datas ou afirmações institucionais que não tenham sido validados pelo projeto.

### 4.4 Atividades Realizadas

Exibir uma galeria de registros fotográficos e audiovisuais das atividades, agrupados por categoria.

**Filtros disponíveis:**

- Todas
- Papo Terreiro
- Roda - Exu
- Roda - Mulher
- Dança
- Roda - Jurema
- Oficina de Costura
- Tear da Visão

**Comportamento dos filtros e da galeria:**

- “Todas” aparece selecionado inicialmente e mostra todos os itens publicados.
- Selecionar uma categoria mostra apenas os itens daquela categoria e atualiza visualmente o filtro selecionado.
- Os filtros podem ser usados por teclado e leitor de tela; seu estado selecionado deve ser anunciado.
- Cada item contém mídia, categoria e, quando fornecidos, título, legenda, data e texto alternativo.
- Se uma categoria não tiver itens publicados, apresentar uma mensagem de estado vazio clara, sem deixar a área em branco.
- Os cards têm affordance visual de abertura e estado de hover sem depender exclusivamente do hover para comunicar a ação.

**Lightbox / visualização ampliada:**

- Abrir a foto ou o vídeo selecionado em uma camada sobre a página.
- Oferecer controle para fechar, além de fechar com `Escape` e, se apropriado, ao clicar fora do conteúdo.
- Permitir navegação entre mídias adjacentes quando existir mais de um item visível; identificar os controles com rótulos acessíveis.
- Em imagens, mostrar a versão ampliada e sua legenda disponível. Em vídeos, oferecer controles de reprodução nativos ou equivalentes acessíveis.
- Manter foco dentro do lightbox enquanto estiver aberto; ao fechar, devolver o foco ao card que o abriu.
- Respeitar a preferência do visitante por movimento reduzido e não iniciar áudio automaticamente.

### 4.5 Atendimentos & Consultas

Apresentar dois cards, com nome, modalidades e ação de agendamento.

**Jorge Roseno:** Búzios, Cartas Ciganas, Quebra de Maldições Familiares, Biomagnetismo e Campo Sistêmico.  
**Vinicius Santos:** Tarot e Baralho Cigano.

Cada card inclui botão de agendamento direto via WhatsApp. O link abre uma conversa com o número oficial correspondente e pode incluir uma mensagem inicial identificando o atendimento selecionado. A mensagem deve ser editável pelo visitante antes do envio.

Os contatos oficiais confirmados são Jorge Roseno (`5581999313741`) e Vinicius Santos (`5581986888709`). Ambos atendem no Riomar Trade Center, Torre 4, 12º andar, sala 1210. As mensagens iniciais estão definidas no site e podem ser editadas pelo visitante antes do envio. A disponibilidade dos atendimentos não é presumida.

O destino de cada link usa `wa.me`, abre em nova aba com `rel="noopener noreferrer"` e tem rótulo acessível que identifica o profissional. Os números e mensagens iniciais ficam juntos em um único objeto de configuração no JavaScript.

### 4.6 Loja / Livro Raízes do Corpo

Apresentar o livro *Raízes do Corpo* com:

- Imagem oficial da capa e texto alternativo descritivo.
- Título e autoria de Jorge Roseno de Ogum.
- Botão “Comprar com Pix” que abre um modal com QR Code BR Code, código Pix copia e cola, controle para copiar o código e ação para enviar o comprovante pelo WhatsApp.
- Valor confirmado: R$ 70,00. Recebedor: Jorge Roseno dos Santos; chave Pix: `+5581999777069`; cidade: Recife.
- Payload Pix montado conforme o BR Code do Banco Central a partir do objeto `CONFIG`, incluindo geração e validação CRC16. O WhatsApp de comprovante usa o telefone da chave Pix e pode ser alterado no mesmo objeto.

Disponibilidade, frete e condições de entrega só devem ser exibidos se forem informados e mantidos atualizados pelo projeto. Não indicar que a compra foi concluída antes da confirmação do pagamento.

### 4.7 Contato e rodapé

O link “Contato” do menu leva à área de contato no rodapé. O rodapé deve incluir:

- Link para o Instagram `@axe.cria`.
- Área para as logomarcas oficiais dos apoiadores e financiadores, com proporção preservada e textos alternativos quando necessário.
- Crédito obrigatório ao financiamento público, identificando a **Chamada Pública Edital Mãe Gilda de Ogum da Fundação Oswaldo Cruz (Fiocruz)** e o **Ministério da Igualdade Racial — Governo Federal**.

Texto institucional sugerido, a confirmar com as regras de aplicação dos selos: **“Projeto realizado com apoio da Chamada Pública Edital Mãe Gilda de Ogum, da Fundação Oswaldo Cruz (Fiocruz), e do Ministério da Igualdade Racial — Governo Federal.”** Se houver texto ou assinatura visual oficial do edital, usar a versão oficial aprovada no lugar desta redação sugerida.

## 5. Requisitos transversais

### Responsividade

- A página deve funcionar em celular, tablet e desktop, sem rolagem horizontal indevida.
- Menu, filtros, cards, mídia ampliada e botões devem permanecer utilizáveis por toque em telas estreitas.
- Imagens devem se adaptar ao espaço disponível sem distorção; priorizar carregamento eficiente de imagens fora da primeira tela.

### Acessibilidade

- Usar estrutura semântica, um título principal (`h1`) e hierarquia de títulos consistente.
- Garantir navegação por teclado, foco visível, rótulos acessíveis e contraste suficiente.
- Fornecer texto alternativo para imagens informativas; imagens decorativas devem ser ignoradas por tecnologias assistivas.
- Não transmitir informação apenas por cor, animação ou hover.
- Respeitar `prefers-reduced-motion`; rolagem suave não deve prejudicar visitantes que desativaram animações.
- O menu móvel e o lightbox devem gerir foco e estado acessível corretamente.

### Desempenho, privacidade e segurança

- Otimizar imagens e vídeos para web; evitar carregamento antecipado de toda a galeria.
- Usar HTTPS na publicação e links externos confiáveis.
- Não coletar dados pessoais nem instalar rastreamento sem necessidade, aviso e base legal definidos pelo projeto.
- Se futuramente houver formulário, definir finalidade, campos, armazenamento, acesso e aviso de privacidade antes de publicá-lo.

### Busca e compartilhamento

- Definir título da página, descrição e imagem de compartilhamento coerentes com a iniciativa.
- Incluir idioma `pt-BR` e conteúdo textual indexável para as informações institucionais essenciais.
- Fornecer URLs/âncoras estáveis para as seções principais.

## 6. Requisitos funcionais resumidos

| ID | Requisito | Critério de aceite |
| --- | --- | --- |
| RF-01 | Navegação por seção | Cada item do menu, o indicador de rolagem e os links internos levam à seção correta sem ocultar seu título sob o cabeçalho fixo. |
| RF-02 | Menu responsivo | Em viewport estreita, o menu abre e fecha por toque e teclado, anuncia seu estado e permite chegar a todos os destinos. |
| RF-03 | Filtro da galeria | Cada categoria filtra os itens correspondentes; “Todas” restaura a galeria completa e categoria sem conteúdo exibe estado vazio. |
| RF-04 | Visualização de mídia | Selecionar um item abre o lightbox; fechar por controle ou `Escape` devolve o foco ao item de origem. |
| RF-05 | Agendamento | Cada profissional tem botão de WhatsApp associado ao contato correto e identificável; nenhum link fictício é publicado. |
| RF-06 | Livro | Capa, sinopse e ação de compra/pedido são apresentados; a ação aponta apenas para canal oficial configurado. |
| RF-07 | Créditos | Rodapé identifica o Edital Mãe Gilda de Ogum, a Fiocruz e o Ministério da Igualdade Racial — Governo Federal, usando selos oficiais aprovados quando fornecidos. |
| RF-08 | Acesso ao Instagram | Links para `@axe.cria` estão disponíveis no cabeçalho e no rodapé e têm nome acessível. |
| RF-09 | Layout adaptável | Conteúdo e controles permanecem utilizáveis em telas pequenas e grandes, sem sobreposição ou corte de texto. |

## 7. Conteúdo e materiais necessários

Antes da publicação, reunir e aprovar:

- Logomarcas horizontal e circular da Axé Cria em formatos adequados para web.
- Arquivos da Alekan Rounded e confirmação de licença para uso na web.
- Fotografias e vídeos das atividades, com categoria, legenda, créditos, autorização de uso e texto alternativo.
- Texto institucional e biografia aprovados, incluindo informações históricas que possam ser publicadas.
- Foto e identificação aprovadas de Jorge Roseno e Vinicius Santos, caso sejam usadas.
- Números oficiais de WhatsApp e mensagens iniciais desejadas para cada profissional.
- Capa, sinopse, preço e disponibilidade de *Raízes do Corpo*, além do canal oficial de compra ou pedido.
- Logomarcas, regras de aplicação e redação oficial do Edital Mãe Gilda de Ogum, Fiocruz, Ministério da Igualdade Racial e Centro Daruê Malungo.
- Confirmação de quais canais de contato devem aparecer além do Instagram e WhatsApp.

## 8. Fora do escopo inicial

- Sistema interno de gestão de conteúdo, usuários ou permissões.
- Agendamento com calendário, confirmação automática, pagamento ou gestão de disponibilidade.
- Checkout, cálculo de frete, processamento de pagamento e gestão de estoque.
- Cadastro de visitantes, comentários ou envio de formulário, salvo decisão posterior.
- Produção de conteúdo, fotografia, vídeo, identidade de marca ou criação de logomarcas institucionais.

## 9. Pendências para aprovação

1. Fornecer os arquivos oficiais da marca, fonte, fotos, vídeos e textos finais.
2. Confirmar a disponibilidade de cada atendimento.
3. Definir disponibilidade, frete e demais condições de entrega do livro.
4. Validar o texto de financiamento e fornecer os selos/logomarcas oficiais e suas regras de uso.
5. Confirmar créditos, autorizações de imagem e informações de contato adicionais.
6. Aprovar a ordem final, os textos e os critérios de publicação das atividades na galeria.
