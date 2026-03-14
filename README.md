@import url('https://fonts.googleapis.com/css2?family=Racing+Sans+One&family=Space+Grotesk:wght@300;400;700&display=swap');
@import "tailwindcss";

@theme {
  --color-brand-orange: #FF6321;
  --color-brand-dark: #050505;
  --color-brand-gray: #111111;
  
  --font-sans: "Space Grotesk", ui-sans-serif, system-ui, sans-serif;
  --font-display: "Racing Sans One", sans-serif;
}

@layer base {
  body {
    @apply bg-brand-dark text-white font-sans antialiased;
  }
}

.glass-card {
  @apply bg-white/5 backdrop-blur-xl border border-white/10 rounded-2xl;
}

.orange-gradient {
  background: linear-gradient(135deg, #FF6321 0%, #FF3D00 100%);
}

.text-stroke {
  -webkit-text-stroke: 1px rgba(255, 255, 255, 0.2);
  color: transparent;
}

@keyframes marquee {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

.animate-marquee {
  animation: marquee 30s linear infinite;
}
