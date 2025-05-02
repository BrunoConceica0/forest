Como fazer a instalação do Vue3 e Tailwindcss 4 Vite

#1 instalação base do Vite
npm init vite my-project

#2 Vai na pasta criado do seu projeto 'cd.. my-project' em seguincia coloque no terminal
npm install

#3 Instalação base do tailwind no terminal
npm install tailwindcss @tailwindcss/vite
teste o npm run dev para ver se esta funcionado

#4 no style.css limpe do os estilos e colcoque somente a importação do tailwindcss
@import "tailwindcss";

#5 No Arquivo vite.config.js faça configuração para tailwindcss e verifique se o main.js esta importando o arquivo style.css
import { defineConfig } from 'vite'

# import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
plugins: [

# tailwindcss(),

],
})
