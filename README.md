## 1 - Quais são as entidades necessárias?

As entidades necessárias são:
Tecnologia
EmpresaParceira
EmpresaTecnologia (tabela de associação entre empresas parceiras e tecnologias)
Colaborador

## 2 - Quais são os principais campos e seus respectivos tipos?

![diagrama](https://github.com/WashLigel/projeto_individual_m2_Resilia_data/blob/main/img%20diagram.PNG)

Para a entidade Tecnologia:
Id: int (chave primária)
Nome: char(50)
Área: char(50)
Para a entidade EmpresaParceira:
Id: int (chave primária)
Nome: char(50)
Para a tabela de associação EmpresaTecnologia:
EmpresaId: int (chave estrangeira referenciando a tabela EmpresaParceira)
TecnologiaId: int (chave estrangeira referenciando a tabela Tecnologia)
Para a entidade Colaborador:
Id: int (chave primária)
Nome: char(50)
EmpresaId: int (chave estrangeira referenciando a tabela EmpresaParceira)
Email: char(50)

## 3 - Como essas entidades estão relacionadas?

A tabela EmpresaTecnologia atua como uma tabela de associação entre as empresas parceiras e as tecnologias que elas utilizam.

Cada entrada na tabela EmpresaTecnologia associa uma empresa parceira a uma tecnologia específica que ela utiliza.

A tabela Colaborador está relacionada com a tabela EmpresaParceira, indicando em qual empresa o colaborador trabalha.


## 4 -Simule 2 registros para cada entidade:

Tecnologia:
Id: 1, Nome: "Python", Área: "Desenvolvimento Web"
Id: 2, Nome: "SQL", Área: "Banco de Dados"
EmpresaParceira:
Id: 1, Nome: "Empresa A"
Id: 2, Nome: "Empresa B"
EmpresaTecnologia:
EmpresaId: 1, TecnologiaId: 1
EmpresaId: 2, TecnologiaId: 2
Colaborador:
Id: 1, Nome: "João Silva", EmpresaId: 1, Email: "joao.silva@empresa.com"
Id: 2, Nome: "Maria Santos", EmpresaId: 2, Email: "maria.santos@empresa.com"
