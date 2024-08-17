def perguntar_sobre_curso():
    # Pergunta sobre o nome do curso
    nome_curso = input("Qual é o nome do curso? ")

    # Pergunta sobre o preço do curso
    preco_curso = input("Quanto custa o curso? ")

    # Pergunta sobre a duração do curso
    duracao_curso = input("Qual é a duração do curso (em meses, semanas ou horas)? ")

    # Pergunta sobre os dias da semana
    dias_semana = input("Quais dias da semana o curso é ministrado? ")

    # Exibe as informações coletadas
    print("\nInformações do Curso:")
    print(f"Nome do Curso: {nome_curso}")
    print(f"Preço do Curso: {preco_curso}")
    print(f"Duração do Curso: {duracao_curso}")
    print(f"Dias da Semana: {dias_semana}")

    # Pergunta se o usuário deseja se inscrever
    inscricao = input("\nVocê deseja se inscrever neste curso? (sim/não): ").strip().lower()

    if inscricao == 'sim':
        nome_usuario = input("Por favor, insira seu nome completo: ")
        email_usuario = input("Por favor, insira seu e-mail: ")
        print(f"\nObrigado, {nome_usuario}! Você se inscreveu com sucesso no curso {nome_curso}.")
        print(f"Um e-mail de confirmação será enviado para {email_usuario}.")
    else:
        print("Você optou por não se inscrever no curso. Obrigado por seu interesse!")
