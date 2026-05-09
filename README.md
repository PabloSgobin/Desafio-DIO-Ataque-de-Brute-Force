# 🔐 Simulação de Ataques de Força Bruta  
### ⚔️ Kali Linux + Medusa + Metasploitable 2

<p align="center">
  <img src="https://img.shields.io/badge/status-concluído-success?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/foco-cybersecurity-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/ferramenta-medusa-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/ambiente-lab%20controlado-yellow?style=for-the-badge"/>
</p>

---

## 🎬 Demonstração

<p align="center">
  <!-- Substitua pelo seu próprio GIF -->
  <img src="https://media.giphy.com/media/26tn33aiTi1jkl6H6/giphy.gif" width="600"/>
</p>

---

## 📌 Sobre o Projeto

Este projeto demonstra, na prática, como ataques de **força bruta** podem comprometer sistemas vulneráveis.

Utilizando um ambiente controlado com **Kali Linux** e **Metasploitable 2**, foram executados ataques simulados em diferentes serviços, evidenciando riscos reais de segurança.

---

## 🎯 Objetivos

✔️ Entender ataques de força bruta  
✔️ Explorar vulnerabilidades reais  
✔️ Utilizar ferramentas de pentest  
✔️ Documentar processos técnicos  
✔️ Aplicar boas práticas de segurança  

---

## 🧪 Ambiente de Testes

| Máquina           | Função       |
|------------------|-------------|
| 🐉 Kali Linux     | Atacante     |
| 🎯 Metasploitable | Alvo         |

**Configuração de rede:**  

Host-Only (rede isolada)
---

## 🛠️ Ferramentas

- Kali Linux  
- Medusa  
- Nmap  
- DVWA  
- Metasploitable 2  

---

## 🔍 Etapas do Ataque

### 🔎 Reconhecimento

```bash
nmap -sV <IP_ALVO>
```
🔐 Força Bruta em FTP
```
medusa -h <IP_ALVO> -u ftp -P wordlist.txt -M ftp
```
💥 Resultado: credenciais encontradas com sucesso

---

🌐 Ataque em Aplicação Web (DVWA)
```
medusa -h <IP_ALVO> -U users.txt -P passwords.txt -M http
```
💥 Resultado: login comprometido via credenciais fracas

---

🖥️ Password Spraying em SMB
```
medusa -h <IP_ALVO> -U users.txt -p senha123 -M smbnt
```
💥 Resultado: usuários vulneráveis identificados
---
## 📊 Resultados Obtidos
- 🔓 Acesso não autorizado obtido
- 🔑 Senhas fracas exploradas
- ⚠️ Falhas de segurança evidenciadas



## 🛡️ Medidas de Mitigação
- ✔️ Senhas fortes e complexas
- ✔️ Bloqueio após tentativas inválidas
- ✔️ Autenticação multifator (MFA)
- ✔️ Monitoramento de logs
- ✔️ Restrição de acesso por IP

---

# ⚠️ Aviso Legal

Este projeto foi realizado apenas para fins educacionais, em ambiente controlado.
Qualquer uso indevido dessas técnicas é ilegal.

---

🚀 Conclusão

Este laboratório mostra como sistemas mal configurados podem ser facilmente comprometidos — e reforça a importância de práticas sólidas de segurança.

---

🧠 Aprendizados
- 💡 Ataques simples podem ser extremamente eficazes
- 💡 Segurança básica ainda é negligenciada
- 💡 Monitoramento é essencial
