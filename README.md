# -AEP---Sistema-de-Gerenciamento-do-Programa-Sa-de-na-Escola---PSE

**Integrantes:**

* Gabriel Henrique de Assis Terres — RA: 26011306-2
* Enzo Hisao Yamamoto Ribeiro — RA: 26007653-2
* Arthur de Freitas Alves — RA: 26006277-2

**Descrição do Projeto:**

Este projeto foi desenvolvido como parte da **AEP do 2º semestre do curso de Engenharia de Software**, tendo como proposta o desenvolvimento de um sistema para o gerenciamento do Programa Saúde na Escola (PSE).

O Programa Saúde na Escola tem como finalidade integrar ações de educação e saúde, contribuindo para o desenvolvimento integral dos estudantes da rede pública de educação básica.

A proposta do projeto surgiu a partir da identificação de dificuldades relacionadas ao acompanhamento e à organização das ações realizadas pelo PSE. Entre essas dificuldades estão a falta de padronização dos registros, a comunicação entre as equipes e a utilização de anotações ou planilhas isoladas.

Para solucionar esse problema, o grupo propõe o desenvolvimento de uma aplicação computacional em **linguagem C**, executada em modo terminal, destinada ao gerenciamento de informações coletivas relacionadas às ações do programa.

O sistema permitirá realizar o **cadastro de ações**, contendo informações como código, escola, tema, data prevista, público-alvo, responsável e quantidade prevista de participantes.

Também será possível **listar e pesquisar ações cadastradas**, utilizando filtros como código, escola ou tema, facilitando a localização das informações necessárias.

Outra funcionalidade será a possibilidade de **atualizar a situação das ações**, classificando-as como planejadas, realizadas ou canceladas. Quando uma ação for realizada, o sistema poderá registrar a quantidade efetiva de participantes.

Além disso, o software contará com um **resumo geral das ações**, permitindo visualizar informações como o total de ações por situação, a quantidade de participantes previstos e efetivos e a taxa percentual de adesão.

O desenvolvimento do projeto também busca aplicar, na prática, conhecimentos adquiridos durante o curso de **Engenharia de Software**, especialmente conceitos relacionados ao levantamento de requisitos, modelagem, algoritmos, fluxogramas, programação, validação e testes.

Por fim, o sistema foi planejado considerando a **privacidade e a proteção dos dados**, não armazenando nomes de estudantes, diagnósticos, prontuários ou informações clínicas individuais. Dessa forma, o projeto mantém seu foco no acompanhamento coletivo das ações do PSE.

programa
{
	funcao inicio()
	{
		inteiro codigo
		cadeia escola
		cadeia tema
		cadeia data_prevista
		inteiro qtd_prevista

		escreva("====================================\n")
		escreva("    CADASTRO DE AÇÃO DO PSE        \n")
		escreva("====================================\n")

		escreva("Digite o código da ação: ")
		leia(codigo)

		escreva("Digite o nome da escola: ")
		leia(escola)

		escreva("Digite o tema da ação: ")
		leia(tema)

		escreva("Digite a data prevista (DD/MM/AAAA): ")
		leia(data_prevista)

		escreva("Digite a quantidade prevista de participantes: ")
		leia(qtd_prevista)

		enquanto (qtd_prevista <= 0)
		{
			escreva("Erro! A quantidade deve ser maior que zero.\n")
			escreva("Digite a quantidade prevista novamente: ")
			leia(qtd_prevista)
		}

		escreva("\n====================================\n")
		escreva("    AÇÃO CADASTRADA COM SUCESSO!    \n")
		escreva("====================================\n")
		escreva("Código: ", codigo, "\n")
		escreva("Escola: ", escola, "\n")
		escreva("Tema: ", tema, "\n")
		escreva("Data: ", data_prevista, "\n")
		escreva("Participantes Previstos: ", qtd_prevista, "\n")
		escreva("Situação Inicial: Planejada\n")
	}
}
