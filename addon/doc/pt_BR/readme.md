# Loja de Complementos para NVDA

> **⚠️ Aviso importante para testadores da versão beta:**
> Se você esteve testando o complemento **TiendaNVDA_Modern**, por favor, **desinstale-o antes de instalar esta versão**. Aquela versão era uma versão de testes e beta que não deve coexistir com esta versão final. Para desinstalá-lo, vá ao menu do NVDA → Ferramentas → Loja de complementos, selecione "TiendaNVDA_Modern" e exclua-o. Reinicie o NVDA e depois proceda com a instalação desta nova versão.

Loja Unificada de Complementos para NVDA: integra a **Loja da Comunidade Hispanofalante (NVDA.ES)** e a **Loja Oficial da NV Access** em uma única interface acessível.

**Autor:** Héctor J. Benítez Corredera  
**Licença:** GNU General Public License v2  
**Versão:** 2026.05.09  
**Compatibilidade:** NVDA 2025.1 a NVDA 2026.1  
**Repositório:** [https://github.com/hxebolax/Tienda-para-NVDA](https://github.com/hxebolax/Tienda-para-NVDA)

---

## Índice

1. [Introdução](#introduccion)
2. [Instalação](#instalacion)
3. [Primeiros passos](#primeros-pasos)
4. [As três lojas](#las-tres-tiendas)
5. [A interface da loja](#la-interfaz-de-la-tienda)
6. [Indicadores de status](#indicadores-de-estado)
7. [Teclas de atalho e funções especiais](#teclas-rapidas-y-funciones-especiales)
8. [Menu de contexto](#menu-contextual)
9. [Gerenciamento de complementos instalados](#gestion-de-complementos-instalados)
10. [Empacotador de complementos](#empaquetador-de-complementos)
11. [Buscar atualizações](#buscar-actualizaciones)
12. [Painel de opções](#panel-de-opciones)
13. [Sistema de cache](#sistema-de-cache)
14. [Modo offline](#modo-offline)
15. [Backup e restauração](#backup-y-restauracion)
16. [Tradução de descrições](#traduccion-de-descripciones)
17. [Servidores personalizados](#servidores-personalizados)
18. [Observações e proteções](#observaciones-y-protecciones)
19. [Resumo de teclas de atalho](#resumen-de-teclas-rapidas)
20. [Colaboradores](#colaboradores)
21. [Registro de alterações](#registro-de-cambios)

---

<a name="introduccion"></a>

## Introdução

A **Loja de Complementos para NVDA** é uma evolução completa da antiga Loja para NVDA.ES, remodelada do zero para oferecer uma experiência moderna, rápida e unificada.

### O que há de novo em relação à versão anterior?

- **Loja Unificada:** Navegue pelos complementos da NVDA.ES e pela loja oficial da NV Access a partir de uma única janela.
- **Indicadores de status:** Cada complemento mostra seu status em tempo real: instalado, atualizável, desabilitado, incompatível, etc.
- **Gerenciamento local:** Desabilite, habilite ou desinstale complementos sem sair da loja.
- **Sistema de cache multinível:** Cache de servidores, cache de traduções e cache de listas para um carregamento ultrarrápido.
- **Modo offline:** Navegue pela loja sem conexão com a internet usando dados armazenados em cache.
- **Backup e restauração:** Crie cópias de segurança dos seus complementos e restaure-os ao mudar de computador.
- **Empacotador:** Gere arquivos `.nvda-addon` a partir de qualquer complemento instalado.
- **Instalação silenciosa:** Instale complementos em segundo plano sem diálogos intermediários.
- **Reinicialização inteligente:** A loja detecta se algo foi realmente instalado antes de solicitar a reinicialização.
- **Verificação de dependências:** Verifica se as dependências do complemento estão atendidas antes de instalar.
- **Tradução com cache:** Traduza descrições instantaneamente com a tecla F3, e as traduções são salvas para não repetir a consulta.
- **Notificações aprimoradas:** As notificações de atualização agora indicam a origem (NVDA.ES ou Oficial) e os nomes os complementos.

---

<a name="instalacion"></a>

## Instalação

1. Baixe o arquivo `.nvda-addon` a partir da página de [releases do repositório](https://github.com/hxebolax/Tienda-para-NVDA/releases).
2. Abra o arquivo baixado ou arraste-o sobre a janela do NVDA.
3. Aceite a instalação quando o NVDA solicitar.
4. Reinicie o NVDA para ativar o complemento.

---

<a name="primeros-pasos"></a>

## Primeiros passos

O complemento vem **sem atalhos de teclado atribuídos**. Você pode atribuir atalhos personalizados a partir de:

**Menu do NVDA → Preferências → Definir comandos... → Loja de Complementos NVDA**

Aqui você encontrará as seguintes ações disponíveis:

- Mostrar a janela com todos os complementos do NVDA.ES
- Buscar atualizações dos complementos instalados no NVDA.ES
- Mostrar a janela com todos os complementos da loja oficial
- Buscar atualizações dos complementos oficiais
- Mostrar a loja unificada com todas as fontes de complementos

### Acesso a partir do menu

Você também pode acessar todas as funções a partir do menu do NVDA:

**Menu NVDA → Ferramentas → Loja de Complementos NVDA**

Aqui você encontrará os seguintes submenus:

- **Loja NVDA.ES:** Listagem de complementos e busca de atualizações da comunidade hispanofalante.
- **Loja Oficial NVDA:** Listagem de complementos e busca de atualizações da loja oficial.
- **Loja Unificada (Todas as fontes):** Mostra todos os complementos de todas as fontes em uma única lista.
- **Empacotador de complementos:** Permite empacotar complementos instalados como arquivos `.nvda-addon`.
- **Documentação do complemento:** Abre esta documentação no navegador padrão.

---

<a name="las-tres-tiendas"></a>

## As três lojas

A nova versão integra três modos de visualização de complementos:

### Loja NVDA.ES

É a loja da comunidade hispanofalante. Obtém os complementos do servidor de [https://nvda.es](https://nvda.es) e de qualquer servidor personalizado que você tenha adicionado.

### Loja Oficial NVDA

Acesse a loja oficial de complementos da NV Access ([https://addons.nvda-project.org](https://addons.nvda-project.org)). Os complementos desta fonte são obtidos diretamente da API da loja oficial e são exibidos com todas as suas informações de compatibilidade.

### Loja Unificada

É a visualização combinada que mostra **todos os complementos de todas as fontes** em uma única lista. Os complementos são identificados com as etiquetas `[ES]` (comunidade hispanofalante) e `[OF]` (loja oficial) para que você saiba de onde vem cada um.

---

<a name="la-interfaz-de-la-tienda"></a>

## A interface da loja

Ao abrir qualquer uma das lojas, é exibida uma janela dividida em dois painéis:

### Painel esquerdo (zona de trabalho)

1. **Caixa de pesquisa:** Ao abrir a loja, o foco é colocado aqui. Digite qualquer termo e pressione Enter para filtrar a lista. Para exibir todos os complementos novamente, limpe o campo de pesquisa e pressione Enter com o campo vazio.

2. **Lista de complementos:** Mostra todos os complementos disponíveis com seu indicador de status entre colchetes (ex: `[I]`, `[U]`). Navegue com as setas Para Cima/Para Baixo.

3. **Botão de ação (Instalar/Atualizar):** Este botão é dinâmico; altera seu texto automaticamente de acordo com o status do complemento selecionado:
   - Se você não tiver o complemento instalado, mostra **"Instalar"**.
   - Se houver uma atualização disponível, mostra **"Atualizar"**.

### Painel direito (ficha informativa)

À medida que você se move pela lista de complementos, este painel é preenchido com as informações completas do complemento selecionado:

- Nome e resumo
- Versão disponível no servidor
- Versão instalada (se aplicável)
- Autor
- Descrição completa
- Compatibilidade com o NVDA (versão mínima e última testada)
- Número de downloads (quando disponível)
- Status da instalação

---

<a name="indicadores-de-estado"></a>

## Indicadores de status

Ao mover-se pela lista de complementos, o NVDA anunciará algumas letras entre colchetes que indicam o status de cada complemento:

| Indicador | Significado                                                                                                             |
| :-------- | :---------------------------------------------------------------------------------------------------------------------- |
| **[I]**   | **Instalado:** O complemento está instalado e ativo.                                                                    |
| **[U]**   | **Atualização:** Há uma nova versão disponível. Atualize!                                                               |
| **[U-I]** | **Atualização incompatível:** Há uma nova versão, mas ela não é compatível com a sua versão do NVDA.                    |
| **[D]**   | **Desativado:** O complemento está instalado, mas foi desativado manualmente.                                           |
| **[R]**   | **Pendente para remoção:** Será removido ao reiniciar o NVDA.                                                           |
| **[I-I]** | **Instalado incompatível:** O complemento está instalado, mas bloqueado por incompatibilidade com a sua versão do NVDA. |
| **[X]**   | **Não compatível:** O complemento não é compatível com a sua versão do NVDA.                                            |

Na **Loja Unificada** também é exibida a procedência:

| Etiqueta | Procedência                                       |
| :------- | :------------------------------------------------ |
| **[ES]** | Servidores do NVDA.ES (comunidade hispanofalante) |
| **[OF]** | Loja oficial da NV Access                         |

---

<a name="teclas-rapidas-y-funciones-especiales"></a>

## Teclas de atalho e funções especiais

Estas teclas funcionam quando o foco está na lista de complementos:

### F1 — Posição atual

Pressione **F1** para que o NVDA diga em qual posição da lista você se encontra: "Você está no complemento 15 de 200".

### Ctrl+F1 — Explicar indicador

Não se lembra do que significam os colchetes `[I]` ou `[U]`? Pressione **Ctrl+F1** e o NVDA explicará em linguagem clara o status do complemento selecionado.

### F2 — Ler ficha completa

Pressione **F2** para que o NVDA leia de uma vez só toda a ficha técnica e a descrição do complemento **sem a necessidade de navegar com Tab até o painel direito**. Funciona em todas as lojas.

### F3 — Traduzir descrição

A descrição está em inglês ou outro idioma? Pressione **F3** e a loja a traduzirá para o idioma que você configurou (por padrão, espanhol). Um som será reproduzido no início e no final da tradução.

> **Nota:** Para usar a tecla F3, você deve ativar previamente o tradutor nas opções do complemento. Requer conexão com a internet.

---

<a name="menu-contextual"></a>

## Menu de contexto

Na lista de complementos, pressione a **Tecla Aplicações** (clique com o botão direito ou **Shift+F10**) para exibir o menu de contexto com as seguintes opções:

### Filtros

- **Mostrar todos os complementos:** Mostra a lista completa (opção padrão).
- **Mostrar complementos por compatibilidade de API:** Filtra apenas os complementos compatíveis com uma versão específica do NVDA.
- **Mostrar complementos ordenados por autor:** Ordena a lista pelo nome do autor.
- **Mostrar por downloads do maior para o menor:** Ordena por popularidade.

> **Nota:** Os filtros não são cumulativos. Cada filtro é executado individualmente e o título da janela muda para informar o filtro ativo. As opções de filtro são mantidas enquanto o NVDA não for reiniciado.

### Copiar para a área de transferência

- **Copiar informação:** Copia a ficha completa do complemento selecionado.
- **Copiar link para a página web:** Copia a URL oficial do complemento.
- **Copiar link de download:** Submenu com os canais de desenvolvimento disponíveis para copiar sua URL de download direto.

---

<a name="gestion-de-complementos-instalados"></a>

## Gerenciamento de complementos instalados

Uma das novidades mais poderosas: se um complemento já está instalado, você pode gerenciá-lo **sem sair da loja**.

1. Selecione um complemento marcado como `[I]`, `[D]` ou `[U]` na lista.
2. Pressione a **Tecla Aplicações** (ou clique com o botão direito).
3. No submenu **Gerenciamento do instalado** você encontrará:

- **Desativar / Ativar:** Ativa ou desativa o complemento temporariamente.
- **Desinstalar:** Marca o complemento para remoção (será efetivada ao reiniciar o NVDA).
- **Ver documentação:** Abre a documentação do complemento no navegador. Se houver documentação no seu idioma, ela será aberta no seu idioma; do contrário, no idioma padrão do complemento.

---

<a name="empaquetador-de-complementos"></a>

## Empacotador de complementos

O empacotador permite gerar arquivos `.nvda-addon` a partir de complementos que você já possui instalados. É ideal para:

- Compartilhar um complemento com outra pessoa sem a necessidade de procurá-lo na loja.
- Criar cópias de segurança de complementos específicos.
- Conservar uma versão particular de um complemento antes de atualizá-lo.

**Para empacotar um complemento:**

1. Vá em **Menu NVDA → Ferramentas → Loja de Complementos NVDA → Empacotador de complementos**.
2. Selecione na lista o complemento que deseja empacotar.
3. Escolha o diretório onde deseja salvar o arquivo.
4. O arquivo `.nvda-addon` será gerado automaticamente com o formato: `nome_versão_Gen.nvda-addon`.

---

<a name="buscar-actualizaciones"></a>

## Buscar atualizações

O complemento oferece duas formas de buscar atualizações:

### Busca manual

A partir do menu de ferramentas, selecione **Buscar atualizações** em qualquer uma das lojas (NVDA.ES ou Oficial). Uma janela será exibida com os complementos que possuem atualizações disponíveis.

Nesta janela você pode:

- **Selecionar complementos individualmente:** Use a barra de espaço para marcar/desmarcar.
- **Alt+S:** Selecionar todos os complementos para atualizar.
- **Alt+D:** Desmarcar todos os complementos.
- **Alt+A:** Iniciar a atualização os complementos selecionados.
- **Alt+C / Escape / Alt+F4:** Fechar a janela.

### Verificação automática

Quando você ativa a verificação automática nas opções:

- A loja buscará atualizações em segundo plano de acordo com o intervalo configurado.
- Mostrará uma NOTIFICAÇÃO do sistema indicando quantas atualizações existem e de qual fonte elas vêm.
- A busca é interrompida automaticamente após 10 verificações sem resultados, ou 5 verificações após encontrar atualizações, para não saturar o servidor.

As notificações agora são mais informativas:

```

Foram encontradas 3 atualizações.

* NVDA.ES (2): Complemento A, Complemento B
* Loja Oficial (1): Complemento C

Execute Buscar atualizações de complementos.

```

---

<a name="panel-de-opciones"></a>

## Painel de opções

Acesse a configuração do complemento a partir de:

**Menu NVDA → Preferências → Opções... → Loja de Complementos NVDA**

### A. Loja NVDA.ES

- **Selecione um servidor de complementos:** Escolha o servidor padrão entre os que você configurou.
- **Gerenciar Servidores de complementos:** Abre o gerenciador onde você pode adicionar, editar ou excluir servidores personalizados.

### B. Loja Oficial NVDA

- **Habilitar loja oficial do NVDA:** Ativa ou desativa a integração com a loja oficial da NV Access.
- **Permitir complementos incompatíveis da loja oficial:** Permite tentar instalar complementos marcados como incompatíveis. **Use por sua conta e risco.**

### C. Atualizações

- **Ativar verificação automática de atualizações:** Ativa a busca em segundo plano.
- **Tempo para verificar atualizações:** Escolha o intervalo entre as verificações:
  - 15 minutos, 30 minutos, 45 minutos, 1 hora, 12 horas, 1 dia, 1 semana.
- **Incluir atualizações da loja oficial:** Adiciona as atualizações da loja oficial à verificação automática.

### D. Tradução

- **Ativar tradutor para descrições:** Habilita o uso da tecla F3 para traduzir.
- **Idioma para traduzir descrições:** Escolha entre 12 idiomas: Alemão, Árabe, Croata, Espanhol, Francês, Inglês, Italiano, Polonês, Português, Russo, Turco e Ucraniano.

### E. Opções Gerais

- **Ordenar complementos alfabeticamente:** Ordena a lista de A a Z.
- **Instalar complementos após o download:** Abre o assistente de instalação automaticamente ao terminar o download.
- **Instalar silenciosamente:** Os complementos são instalados em segundo plano sem diálogos intermediários. Apenas pede para reiniciar ao finalizar.
- **Habilitar cache de servidores:** Armazena as listas de complementos no disco para um carregamento mais rápido.
- **Atualizar cache a cada...:** Configura o intervalo de renovação do cache.
- **Usar cache para traduções:** As traduções feitas com F3 são salvas para não repetir a consulta ao Google.
- **Habilitar modo offline:** Permite navegar pela loja sem conexão com a internet, usando os dados salvos em cache.

### F. Backup e restauração

- **Criar Backup de complementos:** Gera um arquivo JSON com a lista de todos os seus complementos instalados.
- **Restaurar a partir de Backup:** Carrega um arquivo de backup e permite reinstalar os complementos listados.

### G. Complementos instalados que estão no servidor

Na parte inferior das opções é exibida uma lista dos seus complementos que também estão no servidor. A partir daqui você pode:

1. Selecionar um complemento e pressionar a **Barra de espaço**.
2. No menu pop-up, escolher o **canal de atualização** (Estável, Beta, Desenvolvimento, etc.) ou **Descartar atualizações** para que a loja pare de avisar sobre esse complemento.

> **Importante:** As alterações só são salvas ao pressionar OK ou Aplicar no diálogo de opções.

---

<a name="sistema-de-cache"></a>

## Sistema de cache

A loja implementa um sistema de cache multinível para maximizar o desempenho:

### Cache de servidores

Armazena as listas de complementos no disco. Quando você abre a loja, se o cache não tiver expirado, ela é carregada diretamente do disco em vez de fazer uma requisição ao servidor.

- É configurado a partir de: **Habilitar cache de servidores** nas opções.
- O intervalo de atualização é configurável.

### Cache de traduções

As traduções realizadas com F3 são salvas em um arquivo JSON persistente. Da próxima vez que você solicitar a mesma tradução, ela será carregada instantaneamente a partir do cache.

- É configurado a partir de: **Usar cache para traduções** nas opções.

### Cache em memória

Além do cache em disco, a loja mantém um cache na memória RAM para as consultas mais frequentes, eliminando completamente o acesso ao disco durante a sessão.

---

<a name="modo-offline"></a>

## Modo offline

O modo offline permite navegar pela loja **sem conexão com a internet**, utilizando os dados armazenados previamente no cache.

Para utilizá-lo:

1. Certifique-se de ter ativado as opções **Habilitar cache de servidores** e **Habilitar modo offline** nas opções.
2. Navegue pela loja pelo menos uma vez com conexão para que o cache seja gerado.
3. Da próxima vez que você abrir a loja sem internet, os dados serão carregados a partir do cache.

> **Nota:** No modo offline você não poderá baixar nem instalar complementos, mas poderá consultar as informações dos complementos que visitou anteriormente.

---

<a name="backup-y-restauracion"></a>

## Backup e restauração

### Criar backup

1. Vá em **Opções... → Loja de Complementos NVDA → Criar Backup de complementos**.
2. Escolha um nome e localização para o arquivo `.json`.
3. Será gerado um arquivo com a lista de todos os seus complementos instalados, incluindo nome, versão e resumo.

### Backup automático ao sair

A loja cria automaticamente um backup ao fechar o NVDA (configurável nas opções).

### Restaurar a partir de backup

1. Vá em **Opções... → Loja de Complementos NVDA → Restaurar a partir de Backup**.
2. Selecione o arquivo `.json` de backup.
3. A loja mostrará um assistente que buscará as versões mais recentes de cada complemento nos servidores e permitirá que você os instale em lote.

> **Ideal para:** Migrar complementos para um novo computador ou recuperar sua configuração após reinstalar o NVDA.

---

<a name="traduccion-de-descripciones"></a>

## Tradução de descrições

A loja inclui um tradutor integrado baseado no Google Tradutor:

1. **Ative o tradutor** a partir das opções do complemento.
2. **Selecione o idioma de destino** (Espanhol por padrão).
3. **Pressione F3** sobre qualquer complemento na lista para traduzir sua descrição.

Características:

- Som de início e fim para indicar que a tradução está sendo realizada.
- As traduções são armazenadas em cache para não repetir consultas.
- A tradução é perdida ao mudar de complemento; pressione F3 novamente se precisar dela de novo.
- Requer conexão com a internet.

---

<a name="servidores-personalizados"></a>

## Servidores personalizados

Você pode adicionar repositórios de complementos de terceiros que usem o formato compatível com o NVDA.ES.

### Adicionar um servidor

1. Vá em **Opções... → Loja de Complementos NVDA → Gerenciar Servidores de complementos**.
2. Pressione **Adicionar**.
3. Insira um nome descritivo e a URL do servidor.
4. Aceite e o servidor aparecerá no seletor de servidores.

### Exemplo: Servidor da comunidade russa

- **Nome:** Comunidade Russa
- **URL:** `https://nvda-addons.ru/get.php?addonslist`

### Mudar de servidor rapidamente

A partir da janela principal da loja NVDA.ES, pressione **Alt+C** ou o botão **Mudar de servidor** para exibir um menu com todos os servidores configurados. A mudança é imediata e temporária (não é salva como padrão até que você a altere nas opções).

> **Nota:** O servidor padrão da comunidade hispanofalante não pode ser modificado nem excluído.

---

<a name="observaciones-y-protecciones"></a>

## Observações e proteções

O complemento inclui múltiplas proteções para garantir uma experiência segura:

1. **Complementos pendentes para desinstalação:** São excluídos automaticamente das verificações de atualização.
2. **Validação de compatibilidade de API:** Mesmo que a versão do servidor seja mais recente, se não for compatível com a sua versão do NVDA, a atualização não será oferecida.
3. **Notificação de erros de instalação:** Se algum complemento não pôde ser atualizado, o seu nome será informado.
4. **Bloqueio após atualização:** A loja não permite buscar mais atualizações se uma atualização já foi realizada e o NVDA ainda não foi reiniciado.
5. **Notificação pós-reinicialização:** Se a verificação automática detectar que o NVDA não foi reiniciado após a atualização, ela emitirá uma notificação de lembrete.
6. **Proteção sem internet:** Se as bibliotecas não puderem ser carregadas por falta de conexão, isso será informado no log do NVDA e avisado com uma mensagem falada ao tentar acessar a loja.
7. **Reinicialização inteligente:** A loja detecta automaticamente se um complemento foi realmente instalado. Se você cancelar o instalador, ela não pedirá para reiniciar desnecessariamente.
8. **Verificação de dependências:** Antes de instalar, verifica se todas as dependências requeridas foram atendidas.

---

<a name="resumen-de-teclas-rapidas"></a>

## Resumo de teclas de atalho

### Janela principal da loja

| Ação                                  | Tecla                         |
| :------------------------------------ | :---------------------------- |
| Ir para a caixa de pesquisa           | `Alt+B`                       |
| Ir para a lista de complementos       | `Alt+L`                       |
| Instalar / Atualizar                  | `Alt+I`                       |
| Ir para as informações do complemento | `Alt+I` (painel direito)      |
| Ir para a página web do complemento   | `Alt+P`                       |
| Mudar de servidor (apenas NVDA.ES)    | `Alt+C`                       |
| Fechar a loja                         | `Alt+S` / `Escape` / `Alt+F4` |

### Na lista de complementos

| Ação                                              | Tecla                            |
| :------------------------------------------------ | :------------------------------- |
| Saber a posição atual na lista                    | `F1`                             |
| Explicar indicador de status                      | `Ctrl+F1`                        |
| Ler ficha completa do complemento                 | `F2`                             |
| Traduzir descrição                                | `F3`                             |
| Menu de contexto (filtros, copiar, gerenciamento) | `Tecla Aplicações` / `Shift+F10` |

### Janela de atualizações

| Ação                             | Tecla                         |
| :------------------------------- | :---------------------------- |
| Selecionar todos os complementos | `Alt+S`                       |
| Desmarcar todos                  | `Alt+D`                       |
| Iniciar atualização              | `Alt+A`                       |
| Fechar janela                    | `Alt+C` / `Escape` / `Alt+F4` |

---

<a name="colaboradores"></a>

## Colaboradores

- Idioma turco (Umut Korkmaz)
- Idioma russo (Valentín N. Kupriyanov)
- Idioma polonês (Kazimierz Parzych)

<a name="registro-de-cambios"></a>

## Registro de alterações

### Versão 2026.05.20

- Corrigido o atualizador silencioso de idiomas do complemento (em fase beta)

Adicionadas as melhorias de Javi Dominguez (PR #1 e #2)

### Versão 2026.05.13

- Corrigido o atualizador silencioso de idiomas do complemento (em fase beta)

### Versão 2026.05.11

- Adicionado um atualizador silencioso de idiomas do complemento (em fase beta)
- Adicionado idioma russo (Valentín N. Kupriyanov)

### Versão 2026.05.10

- Adicionado idioma turco (Umut Korkmaz)

### Versão 2026.05.09

- Primeira versão da Loja Unificada de Complementos para NVDA.
- Integração completa da Loja NVDA.ES e da Loja Oficial da NV Access.
- Novo sistema de indicadores de status: [I], [U], [D], [R], [I-I], [U-I], [X].
- Gerenciamento local de complementos: desativar, ativar e desinstalar sem sair da loja.
- Sistema de cache multinível: cache de servidores, cache de traduções e cache de listas.
- Modo offline: navegação pela loja sem conexão com a internet usando dados armazenados em cache.
- Backup e restauração de complementos instalados.
- Empacotador de complementos: gera arquivos .nvda-addon a partir de complementos instalados.
- Verificação inteligente de dependências e compatibilidade de API.
- Instalação silenciosa com reinicialização inteligente.
- Tradução de descrições com cache persistente via Google Tradutor.
- Suporte para servidores personalizados de complementos.
- Interface com teclas de atalho F1, Ctrl+F1, F2, F3 para acesso rápido às funções.
- Notificações detalhadas indicando a origem das atualizações (ES / Oficial).

### Versões anteriores (Loja para NVDA.ES)

Este repositório continha anteriormente a versão clássica da **Loja para NVDA.ES** (versões 0.1 a 0.10). A partir da versão 2026.05.09, o repositório foi substituído pela nova **Loja Unificada de Complementos para NVDA**, que é uma reescrita completa do complemento.

Se você deseja consultar o código-fonte ou a documentação da versão antiga, pode fazer isso navegando pelo histórico de commits do repositório no GitHub:

1. Vá para [https://github.com/hxebolax/Tienda-para-NVDA](https://github.com/hxebolax/Tienda-para-NVDA).
2. Clique no link de **commits** (ou pressione no contador de commits que aparece na parte superior do repositório).
3. Procure qualquer commit anterior à data de **9 de maio de 2026** para acessar o código e as releases da loja clássica.
4. Uma vez no commit desejado, você pode pressionar **"Browse files"** para ver o estado completo do repositório naquele momento.

Alternativamente, as releases antigas com seus arquivos `.nvda-addon` continuarão disponíveis na seção de [Releases](https://github.com/hxebolax/Tienda-para-NVDA/releases) do repositório, desde que não sejam excluídas manualmente.

---

Aproveite a Loja de Complementos para NVDA!

**Com carinho:** Héctor J. Benítez Corredera.
