# 🚚 TechDelivery – Plataforma de Entregas Locais de Produtos Tecnológicos  

## 📌 Visão Geral  
O **TechDelivery** é uma aplicação que intermedia a **entrega local de produtos tecnológicos e equipamentos/peças**.  
A ideia é conectar **lojistas, técnicos e consumidores finais** a uma rede de entregadores parceiros, garantindo que o produto chegue ao destino de forma rápida, segura e com rastreamento em tempo real.  

---

## 🎯 Objetivos  
- Facilitar o envio e recebimento de produtos tecnológicos dentro de uma região.  
- Reduzir o tempo de entrega de peças e equipamentos essenciais.  
- Oferecer uma alternativa local mais rápida do que transportadoras tradicionais.  
- Garantir rastreabilidade, segurança e comunicação entre todas as partes.  

---

## 🚀 Funcionalidades  

### Para Clientes  
- Cadastro e autenticação.  
- Solicitação de entregas.  
- Rastreio em tempo real.  
- Histórico de pedidos.  
- Avaliação de serviço.  

### Para Lojistas/Técnicos  
- Cadastro de produtos.  
- Gestão de pedidos.  
- Relatórios de vendas e entregas.  

### Para Entregadores  
- Recebimento de notificações.  
- Rotas otimizadas.  
- Confirmação de retirada/entrega.  
- Histórico de entregas.  

---

## 🛠️ Tecnologias  

- **Frontend:** React.js, React Native, TailwindCSS, Mapbox/Google Maps.  
- **Backend:** Node.js + Express, PostgreSQL, Prisma ORM, Redis, JWT.  
- **Infraestrutura:** Docker, Nginx, AWS S3, CI/CD com GitHub Actions.  

---

## 🗂️ Estrutura  

```
techdelivery/
│── backend/         
│   ├── src/
│   ├── prisma/
│   └── tests/
│
│── frontend/        
│   ├── src/
│   └── public/
│
│── mobile/          
│   ├── src/
│   └── assets/
│
│── docs/            
│── docker-compose.yml
│── README.md
```

---

## 🔑 Modelagem de Dados  

- **Usuário** (id, nome, email, senha, tipo)  
- **Produto** (id, nome, descrição, valor, estoque, lojista_id)  
- **Pedido** (id, cliente_id, produto_id, status, origem, destino, entregador_id, criado_em)  
- **Entrega** (id, pedido_id, status, hora_retirada, hora_entrega, comprovante)  

---

## ⚙️ Como Executar  

```bash
# Clonar
git clone https://github.com/seu-usuario/techdelivery.git
cd techdelivery

# Subir containers
docker-compose up -d

# Backend
cd backend
npm install
npx prisma migrate dev
npm run dev
```

API disponível em: `http://localhost:3000`  

---

## 🔮 Futuras Melhorias  
- Pagamentos integrados (Pix/cartão).  
- Cashback e fidelidade.  
- Algoritmo de otimização de rotas.  
- Integração com WhatsApp.  
- Suporte a múltiplas regiões.  

---

## 🤝 Contribuição  
1. Fork o projeto  
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`)  
3. Commit (`git commit -m 'feat: nova funcionalidade'`)  
4. Push (`git push origin feature/nova-funcionalidade`)  
5. Abra um Pull Request  

---

## 📄 Licença  
Licenciado sob **MIT**.
