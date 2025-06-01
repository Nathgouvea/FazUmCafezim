# FazUmCafezim - Website

Site estático de uma única página para a marca brasileira FazUmCafezim, desenvolvido com HTML5, TailwindCSS e JavaScript vanilla.

## 🚀 Tecnologias

- HTML5
- TailwindCSS (via CDN)
- JavaScript Vanilla
- Formspree (para formulários)
- Google Maps Embed API

## 📋 Pré-requisitos

- Conta no GitHub
- Conta no Formspree (para os formulários)
- Imagens e assets do projeto

## 🔧 Configuração

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/fazumcafezim-site.git
cd fazumcafezim-site
```

2. Configure o Formspree:

   - Crie uma conta em [formspree.io](https://formspree.io)
   - Crie dois formulários (um para preferências e outro para contato)
   - Substitua `your-form-id` nos arquivos HTML pelos IDs dos seus formulários

3. Configure o Google Maps:

   - Obtenha uma chave de API do Google Maps
   - Substitua a URL do iframe no arquivo `index.html` pela URL do seu local

4. Adicione as imagens:
   - Coloque todas as imagens na pasta `Imagens/`
   - Certifique-se de que os nomes dos arquivos correspondam aos usados no HTML

## 🚀 Deploy no GitHub Pages

1. Crie um novo repositório no GitHub:

   - Nome: `fazumcafezim-site`
   - Visibilidade: Público

2. Faça o push do código:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/seu-usuario/fazumcafezim-site.git
git push -u origin main
```

3. Configure o GitHub Pages:

   - Vá para Settings > Pages
   - Source: Branch main
   - Folder: / (root)
   - Salve as configurações

4. Aguarde alguns minutos e seu site estará disponível em:
   `https://seu-usuario.github.io/fazumcafezim-site`

## 📝 Notas

- O site é totalmente responsivo
- Todas as imagens devem ser otimizadas para web
- Os formulários são processados via Formspree
- O mapa é carregado via Google Maps Embed API

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
