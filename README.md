# AulaBancoJunto-mySql
-- Criar banco de dados
CREATE DATABASE ProfissoesDB;

-- Usar o banco de dados
USE ProfissoesDB;

-- Criar a tabela com profissões
CREATE TABLE profissao (
    id INT PRIMARY KEY,
    profissao VARCHAR(20),
    experiencia_anos INT,
    projetos_completos INT,
    horas_trabalhadas INT,
    produtividade INT
);

-- Inserir dados na tabela profissao
INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (1, 'Engenheiro', 15, 120, 25000, 85);

-- Selecionar todos os registros da tabela profissao
SELECT * FROM profissao;

-- Inserir mais dados na tabela profissao
INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (2, 'Médico', 20, 200, 30000, 90);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (3, 'Professor', 10, 150, 18000, 75);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (4, 'Advogado', 12, 100, 22000, 80);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (5, 'Desenvolvedor', 8, 90, 16000, 78);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (6, 'Arquiteto', 14, 110, 21000, 82);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (7, 'Designer', 7, 60, 12000, 70);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (8, 'Psicólogo', 9, 50, 13000, 72);

INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (9, 'Enfermeiro', 6, 80, 14000, 74);

-- Inserir dados com erro corrigido
INSERT INTO profissao (id, profissao, experiencia_anos, projetos_completos, horas_trabalhadas, produtividade) 
VALUES (10, 'Consultor', 5, 40, 10000, 65);

-- Selecionar todos os registros da tabela profissao
SELECT * FROM profissao;

-- Excluir o registro onde id = 2 (Médico)
DELETE FROM profissao WHERE id = 2;

-- Atualizar os anos de experiência do Engenheiro (id = 1)
UPDATE profissao SET experiencia_anos = 18 WHERE id = 1;
