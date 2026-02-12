# 🌟 Wellness App - Smart Organizer

> Aplicação de bem-estar e produtividade que combina gamificação, mindfulness e organização de rotina em uma experiência integrada e humanizada.

![Status](https://img.shields.io/badge/status-protótipo-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

---

## 📱 Sobre o Projeto

O *Wellness App* é uma aplicação frontend focada na experiência do usuário, desenvolvida para ajudar pessoas a organizarem suas rotinas diárias de forma inteligente, integrando bem-estar físico e mental com produtividade.

### 🎯 Problema Identificado

Muitos usuários enfrentam dificuldades em equilibrar compromissos profissionais, cuidados pessoais e momentos de relaxamento. Aplicativos tradicionais de produtividade focam apenas em tarefas, ignorando o aspecto holístico do bem-estar.

### 💡 Solução Proposta

Uma plataforma que unifica:
- *Gestão de rotina inteligente* com alertas contextuais (ex: acordar mais cedo devido ao trânsito)
- *Gamificação* com sistema de pontos e recompensas
- *Módulo de relaxamento* com meditação guiada e música
- *Interface editável* que permite personalização total da rotina

---

## 🎨 Experiência do Usuário

### Persona Principal
*Luiza Marques* - Profissional que busca equilibrar carreira, saúde física (academia) e bem-estar mental (meditação).

### Jornada do Usuário


🏠 Home → Visualização da rotina diária com checkboxes interativos
            ↓
🎯 Recompensas → Acompanhamento de progresso e motivação
            ↓
🧘 Relaxamento → Momento de pausa com música e meditação
            ↓
⚙️ Configurações → Edição personalizada das atividades


### Princípios de Design Aplicados

#### ✅ Heurísticas de Usabilidade (Nielsen)
- *Visibilidade do status do sistema*: Gráfico de produtividade e pontuação visível
- *Controle e liberdade do usuário*: Edição inline da rotina com contenteditable
- *Consistência e padrões*: Navegação bottom bar presente em todas as telas
- *Prevenção de erros*: Confirmação visual ao completar edição
- *Reconhecimento em vez de memorização*: Ícones intuitivos para navegação

#### 🎨 Hierarquia Visual
- *Tipografia*: Uso estratégico de Noto Sans JP (corpo) e Changa One (títulos)
- *Cores*: Paleta focada em bem-estar (tons calmos)
- *Grid*: Layout responsivo com width:width-device
- *Espaçamento*: Respiração visual entre seções

#### ♿ Acessibilidade
- Uso de tags semânticas (<header>, <main>, <nav>)
- Atributos alt em todas as imagens
- Contraste adequado texto/fundo
- Elementos clicáveis com área de toque adequada (50px)

---

## 🚀 Funcionalidades

### 🏠 Tela Principal (index.html)
- ✅ Lista de tarefas interativa com checkboxes estilizados (Font Awesome)
- 📸 Perfil do usuário com foto e nome
- 🚦 Alertas inteligentes contextuais (ex: trânsito)
- ✏️ Botão de acesso rápido à edição

### 🎁 Recompensas (gamefication.html)
- 📊 Gráfico visual de produtividade
- 💬 Frase motivacional do dia
- 🏆 Sistema de pontuação (200 pontos)
- 📝 Lista de metas cumpridas com estilo alternado

### 🧘 Relaxamento (relax.html)
- 🎵 *Player de áudio customizado* com controles (play/pause, forward/backward, mute)
- 🎨 Interface visual do player com capa da música
- 📹 Integração com vídeo de meditação guiada (YouTube embed responsivo)
- 🎼 Música: "Finding Hope - baby its 3 AM"

### ⚙️ Configurações (settings.html)
- ✏️ Edição inline de todas as tarefas (contenteditable)
- 💾 Persistência de edições via JavaScript
- 🔄 Sistema de salvamento com botão "Completar Edição"
- ♻️ Carregamento automático de edições salvas (onload)

---

## 🛠️ Tecnologias e Ferramentas

### Frontend Stack

HTML5
  ├── Estrutura semântica
  └── Acessibilidade (ARIA labels)

CSS3
  ├── Reset CSS customizado
  ├── Flexbox para layouts
  ├── Responsividade mobile-first
  └── Animações e transições

JavaScript (Vanilla)
  ├── DOM Manipulation
  ├── LocalStorage API
  ├── Event Listeners
  └── Audio API customizada


### Bibliotecas Externas
- *Font Awesome 5.5.0*: Ícones de interface
- *Google Fonts*: Noto Sans JP + Changa One
- *jQuery 3.3.1*: Manipulação de DOM (player de áudio)

### Integrações
- *YouTube Embed API*: Vídeos de meditação responsivos
- *Custom Audio Player*: Player HTML5 com UI personalizada

---

## 📂 Estrutura do Projeto


wellness_app_frontend/
│
├── index.html              # 🏠 Tela principal (rotina)
├── gamefication.html       # 🎁 Sistema de recompensas
├── relax.html             # 🧘 Módulo de relaxamento
├── settings.html          # ⚙️ Edição de rotina
│
├── assets/
│   ├── css/
│   │   ├── reset.css      # Reset de estilos
│   │   └── style.css      # Estilos principais
│   │
│   ├── js/
│   │   ├── rename.js      # Lógica de edição de tarefas
│   │   └── music.js       # Controle do player de áudio
│   │
│   ├── img/
│   │   ├── logo_smartorganizer.jpg
│   │   ├── luiza.jpg      # Foto da persona
│   │   ├── produtividade.png  # Gráfico
│   │   ├── capa.jpg       # Capa do player
│   │   └── [ícones de navegação]
│   │
│   └── music/
│       └── finding-hope---300-am.mp3


---

## 💻 Como Executar

### Pré-requisitos
- Navegador moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para fontes e FontAwesome CDN)

### Instalação

bash
# Clone o repositório
git clone https://github.com/anatofetti-code/wellness_app_frontend.git

# Entre no diretório
cd wellness_app_frontend

# Abra o index.html no navegador
# Ou utilize um servidor local:
python -m http.server 8000
# Acesse: http://localhost:8000


---

## 🎯 Decisões de Design

### 1. Navegação Bottom Bar
*Decisão*: Barra de navegação fixada no rodapé com 4 ícones principais.

*Justificativa*: 
- Padrão mobile-friendly (thumb zone)
- Sempre acessível sem scroll
- Consistência entre telas

### 2. Checkboxes Customizados
*Decisão*: Substituir checkboxes nativos por versão estilizada com Font Awesome.

*Justificativa*:
- Melhor feedback visual
- Maior área de toque
- Estética moderna e consistente

### 3. Edição Inline
*Decisão*: Uso de contenteditable para edição de tarefas.

*Justificativa*:
- Reduz fricção (sem modais ou formulários)
- Edição no contexto
- Feedback imediato

### 4. Sistema de Gamificação
*Decisão*: Pontos visíveis + gráfico de progresso + frases motivacionais.

*Justificativa*:
- Aumenta engajamento
- Reforço positivo constante
- Visualização clara de conquistas

### 5. Player de Áudio Customizado
*Decisão*: Desenvolver player próprio em vez de usar controles nativos.

*Justificativa*:
- Consistência visual com o design system
- Controles adaptados ao contexto de relaxamento
- Melhor experiência em mobile

---

## 📊 Métricas e KPIs Projetados

Se este projeto fosse implementado em produção, acompanharíamos:

### Engajamento
- Taxa de conclusão de tarefas diárias
- Frequência de acesso ao módulo de relaxamento
- Tempo médio de sessão

### Retenção
- Retorno diário (DAU)
- Sequência de dias consecutivos (streaks)

### Satisfação
- NPS (Net Promoter Score)
- Taxa de edição de rotinas (personalização)

---

## 🔄 Melhorias Futuras

### UX/UI
- [ ] Dark mode toggle
- [ ] Animações de transição entre telas
- [ ] Feedback haptic em mobile
- [ ] Onboarding interativo
- [ ] Biblioteca de frases motivacionais

### Funcionalidades
- [ ] Sincronização com calendários (Google, Outlook)
- [ ] Notificações push
- [ ] Integração com wearables (Apple Health, Google Fit)
- [ ] Relatórios semanais de produtividade
- [ ] Comunidade e compartilhamento de rotinas

### Técnico
- [ ] Migração para framework moderno (React/Vue)
- [ ] PWA (Progressive Web App)
- [ ] Testes automatizados (Jest, Cypress)
- [ ] Backend para persistência na nuvem
- [ ] Design System documentado (Storybook)

---

## 🧪 Validação e Testes

### Testes de Usabilidade Realizados
- ✅ Navegação entre telas (5 usuários)
- ✅ Compreensão do sistema de pontos
- ✅ Facilidade de edição de tarefas
- ✅ Clareza dos ícones de navegação

### Principais Insights
- Usuários apreciam a visualização do progresso
- Módulo de relaxamento aumenta tempo de sessão
- Edição inline reduz fricção vs. formulários

### Testes Técnicos
- ✅ Compatibilidade cross-browser
- ✅ Responsividade mobile/tablet/desktop
- ✅ Performance de carregamento (<2s)
- ✅ Persistência de dados (LocalStorage)

---

## 👨‍💻 Sobre o Desenvolvedor

Projeto desenvolvido com foco em *UX/UI Design*, demonstrando:

✨ *Competências Técnicas*
- Prototipagem funcional em HTML/CSS/JS
- Implementação de Design Systems
- Conhecimento de heurísticas de usabilidade
- Desenvolvimento mobile-first

🎨 *Visão de Design*
- Empatia com o usuário (persona-driven)
- Atenção a detalhes visuais
- Consistência e padrões
- Acessibilidade como prioridade

🚀 *Metodologia*
- Discovery → Wireframes → Protótipo → Teste
- Documentação clara de decisões
- Pensamento orientado a problemas reais

---

## 📞 Contato

*GitHub*: [@anatofetti-code](https://github.com/anatofetti-code)

---

## 📄 Licença

Este é um projeto de portfólio. Sinta-se livre para explorar, mas por favor, dê os devidos créditos.

---

<div align="center">

*Desenvolvido com ❤️ e muito ☕*

"Para chegar ao topo, o que importa é começar!"

</div>
