# 🎬 Player de Vídeo - Atividade 10

## 📖 Sobre o Projeto

Player de vídeo web desenvolvido em **Next.js** como adaptação do player de áudio das atividades anteriores. Este projeto implementa um sistema completo de reprodução de vídeos com controles personalizados e design moderno.

**Disciplina:** Multimídia  
**Atividade:** 10 - Player de Vídeo  
**Desenvolvido por:** Lucas Do Nascimento Rodrigues

---

## 🎯 Objetivo

Adaptar o player de áudio desenvolvido anteriormente para criar um player de vídeo funcional, mantendo a identidade visual do projeto e adicionando recursos específicos para reprodução de vídeo.

---

## ✅ Requisitos Implementados

### ✅ 1. Play e Pause
- [x] Botão play/pause funcional
- [x] Métodos `play()` e `pause()` do HTML5
- [x] Ícone dinâmico que muda conforme o estado
- [x] Clique no vídeo para alternar play/pause
- [x] Botão play central quando pausado

### ✅ 2. Controle de Volume
- [x] Slider de volume (0-100%)
- [x] Botão mute/unmute com ícone dinâmico
- [x] Volume persistente ao desmutar
- [x] Sincronização em tempo real

### ✅ 3. Tag `<video>` HTML5
- [x] Implementação com `<video>` nativo
- [x] Suporte a arquivos `.mp4` locais
- [x] Métodos JavaScript nativos
- [x] Poster/thumbnail enquanto carrega

### ✅ 4. Layout Responsivo
- [x] Design adaptável (mobile/tablet/desktop)
- [x] Grid responsivo com Tailwind CSS
- [x] Controles organizados
- [x] Interface moderna e intuitiva

### ✅ 5. Repositório GitHub
- [x] Código hospedado publicamente
- [x] Estrutura organizada
- [x] README completo
- [x] Comentários no código

---

## 🚀 Funcionalidades

### Controles Principais
- **▶️ Play/Pause**: Iniciar ou pausar reprodução
- **⏮️ Anterior**: Voltar para vídeo anterior
- **⏭️ Próximo**: Avançar para próximo vídeo
- **🔊 Volume**: Ajustar volume com slider (0-100%)
- **🔇 Mute**: Silenciar/reativar som
- **⛶ Fullscreen**: Tela cheia

### Recursos Extras
- **Playlist Visual**: Lista com 3 vídeos
- **Barra de Progresso**: Navegação temporal
- **Auto-hide Controls**: Controles somem após 3s
- **Indicador de Reprodução**: Mostra vídeo atual
- **Informações**: Título e descrição do vídeo
- **Tempo**: Exibição de tempo atual/total

---

## 🛠️ Tecnologias Utilizadas

- **[Next.js 14](https://nextjs.org/)** - Framework React
- **[React 18](https://react.dev/)** - Biblioteca de interface
- **[TypeScript](https://www.typescriptlang.org/)** - Tipagem estática
- **[Tailwind CSS](https://tailwindcss.com/)** - Estilização
- **[Lucide React](https://lucide.dev/)** - Ícones
- **HTML5 Video API** - Controle nativo de vídeo

---

## 📂 Estrutura do Projeto

```
player-video/
├── public/
│   ├── video.mp4           # Vídeo 1
│   ├── video2.mp4          # Vídeo 2
│   ├── video3.mp4          # Vídeo 3
│   ├── thumbnail1.jpg      # Miniatura 1
│   ├── thumbnail2.jpg      # Miniatura 2
│   └── thumbnail3.jpg      # Miniatura 3
├── src/
│   └── app/
│       ├── page.tsx        # Componente do player
│       ├── layout.tsx      # Layout da aplicação
│       └── globals.css     # Estilos globais
├── package.json
├── tsconfig.json
├── tailwind.config.ts
├── next.config.ts
└── README.md
```

---

## 🚀 Como Executar

### Pré-requisitos
- Node.js 18+
- npm ou yarn

### Instalação

```bash
# 1. Clone o repositório
git clone https://github.com/lucasNrodrigues/Atividade-10-play-de-video

# 2. Entre na pasta
cd video-player-multimidia-atividade-10

# 3. Instale dependências
npm install
```

### Executar

```bash
# Modo desenvolvimento
npm run dev

# Acesse: http://localhost:3000
```

### Build para Produção

```bash
npm run build
npm start
```

---

## 🎮 Como Usar

### Controles Básicos
1. **Play/Pause**: Clique no botão ▶️ ou no vídeo
2. **Volume**: Arraste o slider ou clique no ícone 🔊
3. **Navegação**: Use ⏮️ e ⏭️ para trocar vídeos
4. **Progresso**: Arraste a barra vermelha
5. **Tela Cheia**: Clique em ⛶

### Atalhos
- **Espaço**: Play/Pause (quando player focado)
- **Setas**: Navegação temporal
- **F**: Fullscreen
- **M**: Mute

---

## 📱 Responsividade

O player se adapta a diferentes tamanhos de tela:

- **Desktop (>768px)**: Layout com playlist lateral
- **Tablet/Mobile (<768px)**: Layout empilhado
- **Fullscreen**: Controles otimizados

---

## 🎨 Design e Identidade Visual

### Paleta de Cores
- **Primária**: Vermelho (#dc2626) - Lembrando YouTube
- **Secundária**: Cinza escuro (#1f2937)
- **Contraste**: Branco (#ffffff)
- **Fundo**: Gradiente cinza-preto

### Fontes
- **Sistema**: Padrão do Tailwind (sans-serif)

### Elementos
- Controles com hover effects
- Sombras e profundidade
- Animações suaves
- Ícones modernos

---

## 🔧 Personalização

### Adicionar Novos Vídeos

Edite `page.tsx`:

```typescript
const [videos] = useState<Video[]>([
  {
    id: 1,
    title: "Seu Vídeo",
    description: "Descrição do vídeo",
    url: "/seu-video.mp4",
    thumbnail: "/sua-thumbnail.jpg"
  }
]);
```

### Mudar Cores

Edite as classes do Tailwind:

```typescript
// De vermelho para azul
className="bg-red-600" → className="bg-blue-600"
```

---

## 📊 Comparação: Áudio vs Vídeo

| Recurso | Player Áudio | Player Vídeo |
|---------|--------------|--------------|
| Play/Pause | ✅ | ✅ |
| Volume | ✅ | ✅ |
| Progresso | ✅ | ✅ |
| Playlist | ✅ | ✅ |
| **Visual** | ❌ | ✅ |
| **Fullscreen** | ❌ | ✅ |
| **Poster** | ❌ | ✅ |
| **Auto-hide** | ❌ | ✅ |

---

```bash
# Usando SimpleScreenRecorder
simplescreenrecorder

# Configurar:
- Área: Janela do navegador
- Áudio: Microfone
- Duração: Máximo 3 minutos
```

## 🆘 Solução de Problemas

### Vídeo não carrega
- Verifique se arquivo `.mp4` está em `public/`
- Confirme que o nome corresponde ao código
- Teste em outro navegador

### Controles não aparecem
- Mova o mouse sobre o vídeo
- Verifique se JavaScript está habilitado
- Limpe cache do navegador

### Erro de compilação
```bash
rm -rf node_modules .next
npm install
npm run dev
```

---

## 🔗 Links

- **GitHub**: https://github.com/SEU_USUARIO/player-video

---

## 👨‍💻 Autor

**Lucas do Nascimento Rodrigues**

- GitHub: [@lucasNrodrigues](https://github.com/lucasNrodrigues/Atividade-10-play-de-video)
- Email: lr3988506@gmail.com

---

## 📝 Licença

Projeto desenvolvido para fins educacionais.

---

## 🙏 Agradecimentos

- Professor pela orientação
- Comunidade Next.js
- Desenvolvedores das bibliotecas utilizadas

---

## 📌 Notas Importantes

### Requisitos Atendidos
✅ Play/Pause funcional  
✅ Controle de volume  
✅ Tag `<video>` HTML5  
✅ Layout responsivo  
✅ GitHub público  
✅ Vídeo demonstrativo

### Diferenciais
✨ Playlist com múltiplos vídeos  
✨ Controles auto-hide  
✨ Fullscreen  
✨ Design moderno   

---

**⭐ Player de Vídeo - Atividade 10 Completa!**

_Última atualização: Outubro 2024_
