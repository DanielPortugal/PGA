# 🧠 Oracle SQL Scripts – PGA e Cursores

[![Oracle](https://img.shields.io/badge/Oracle-DB-F80000?logo=oracle&logoColor=white)](https://www.oracle.com/database/)  
📖 Coleção de **scripts SQL focados em análise da PGA (Program Global Area)** e monitoramento de **cursores** no Oracle Database.  

Esses scripts são úteis para diagnosticar performance, identificar gargalos e otimizar o uso de memória e cursores no ambiente Oracle.  

---

## 📑 Sumário

- [🎯 consultar_cache_cursor_hits.sql](#-consultar_cache_cursor_hitssql)
- [🔄 consultar_cursores_utilizados.sql](#-consultar_cursores_utilizadossql)
- [📊 consultar_pga_carga_trabalho.sql](#-consultar_pga_carga_trabalhosql)
- [📈 consultar_pga_eficiencia_carga_trabalho.sql](#-consultar_pga_eficiencia_carga_trabalhosql)
- [👤 consultar_pga_sessao_estatisticas.sql](#-consultar_pga_sessao_estatisticassql)

---

## 🎯 consultar_cache_cursor_hits.sql
Analisa a **eficiência do cache de cursores** (Library Cache) no Oracle:  
- Mostra a taxa de reutilização de cursores.  
- Ajuda a identificar problemas com **"hard parsing"** e excesso de cursores abertos.  

---

## 🔄 consultar_cursores_utilizados.sql
Exibe o número de **cursores abertos e utilizados** no banco por sessão:  
- Útil para identificar aplicações que abrem muitos cursores e não fecham corretamente.  

---

## 📊 consultar_pga_carga_trabalho.sql
Gera estatísticas de uso da **PGA** durante diferentes cargas de trabalho:  
- Mostra o consumo total e por sessão.  
- Auxilia no ajuste de parâmetros como `PGA_AGGREGATE_TARGET`.  

---

## 📈 consultar_pga_eficiencia_carga_trabalho.sql
Analisa a **eficiência da PGA** durante cargas de trabalho:  
- Percentual de operações executadas **in-memory**.  
- Identifica se o banco está fazendo **spill para disco** por falta de PGA.  

---

## 👤 consultar_pga_sessao_estatisticas.sql
Mostra estatísticas detalhadas de uso de PGA **por sessão**:  
- Quantidade de memória alocada.  
- Quantidade de memória liberada.  
- Identifica sessões com alto consumo de PGA.  

---

## 🚀 Como usar
📂 Execute os scripts diretamente no **SQL*Plus**, SQLcl, SQL Developer ou qualquer outra ferramenta compatível com Oracle.  

---

## 🛠️ Requisitos
- Oracle Database 11g ou superior.  
- Acesso com privilégios para consultar views de desempenho (`V$` e `GV$`).  

---

## 🤝 Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir um **Pull Request** ou relatar problemas via **Issues**.  

---

## 📄 Licença
Este projeto está licenciado sob a [MIT License](LICENSE).  
