<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="40px" src="https://hermes.digitalinnovation.one/assets/diome/logo-minimized.png"></a>
    <span> Infraestrutura no Azure: VMs, Redes e Disaster Recovery</span>
</h1>

Repositório criado para armazenamento de **resumo e anotações** do curso sobre **infraestrutura na nuvem com Microsoft Azure**, abordando conceitos fundamentais de máquinas virtuais, redes, segurança e estratégias de disaster recovery. Curso oferecido pela [Digital Innovation One](https://www.dio.me/).

---

## 🧠 Conceitos Abordados

### ☁️ Disaster Recovery & Backup

- Estratégia de **replicação de dados entre datacenters** para garantir continuidade de serviço em caso de falhas.
- Armazenamento em servidores alternativos garante **alta disponibilidade** e **resiliência**.

### 📦 Grupo de Recursos

- Um **grupo de recursos** é um **contêiner lógico** que agrupa serviços relacionados (VMs, redes, discos, etc.).
- Permite aplicar **políticas de segurança**, **controle de acesso** (RBAC) e **gerenciamento centralizado**.

### 🖥️ Máquinas Virtuais (VMs)

- Criação de VMs com:
  - **VNet (Virtual Network)** para endereçamento IP e controle de tráfego.
  - **DNS Azure** integrado.
  - **Gateway VPN Site-to-Site**, conectando redes locais ao Azure.
- **Extensões** podem ser instaladas para configurar ou monitorar a VM.
- **Recomendação ativada para "Excluir com VM"** – para evitar resíduos no ambiente.

### 🛡️ Conjuntos de Disponibilidade

- Garante que suas VMs estejam distribuídas em:
  - **Domínios de Atualização** (Update Domains) – evitar downtime durante manutenção.
  - **Domínios de Falha** (Fault Domains) – evitar perda por falha física.
- Segurança por **isolamento de fluxo (Deflow)** entre VMs.

### 📈 Conjuntos de Dimensionamento (Scale Set)

- Permitem criar e gerenciar um conjunto de VMs idênticas.
- Escalabilidade automática com base na demanda (horizontal scaling).

### 🖥️ Área de Trabalho & Pool

- Configurações para **pool de sessões de área de trabalho remota**.
- Ideal para cenários com múltiplos usuários acessando a mesma infraestrutura.

---

## ⚙️ Como Criar uma Máquina Virtual no Azure

1. Acesse o portal Azure.
2. Vá em **Máquinas Virtuais** > **Criar**.
3. Selecione o **grupo de recursos**.
4. Defina:
   - Imagem da VM (Windows/Linux).
   - Tamanho (SKU).
   - Rede virtual e IP.
   - Opções de disponibilidade (conjunto de disponibilidade).
   - Extensões se necessário.
5. Conclua e aguarde a implantação.

---

## 🚀 Extras

- 📡 **VPN Gateway** para conexões seguras entre sua rede local e o Azure.
- 🔁 **Backup automático** e replicação entre regiões.
- 🧩 **DNS Azure** para resolução de nomes dentro da rede virtual.
- 🔐 **Controle de Acesso baseado em função (RBAC)** para gerenciar quem pode fazer o quê.

---

Feito com 💻 por [Rafael Pontes (Bridges)](https://github.com/seu-usuario-aqui) ✨  
