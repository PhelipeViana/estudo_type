npm install typescript ts-node-dev -D
npx tsc --init
#configurar rota no arquivo: tsconfig.json
"baseUrl": "./src",
"paths": {
  "@/*":["./*"]
}

instalar apos para reconhecimento das pastas pelo typescript
npm install tsconfig-paths -D

#configurar npm run dev

"scripts": {
"test": "echo \"Error: no test specified\" && exit 1",
"dev": "ts-node-dev -r tsconfig-paths/register --respawn --quiet --clear ./src/main.ts"
},

Agora é só pau no gato!