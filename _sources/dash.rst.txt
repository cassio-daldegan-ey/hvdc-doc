Dashboard
=========

O dashboard do projeto de previsão de temperatura do HVDC tem como objetivo disponibilizar para o seu usuário um registro do histórico de temperaturas da sala de válvula que estamos monitorando (além de outras variáveis adcionais) assim como a previsão de temperatura para duas semanas futuras.

Para tanto contamos com duas abas:

Visão Geral
-----------

.. figure:: visao_geral.png
    :align: center
    :alt: Aba Visão Geral
    :scale: 50%

As funcionalidades presentes na aba "Visão Geral" são:

* Monitorar os dados históricos de temperatura: série histórica de temperatura das válvulas iniciada em novembro de 2024.
* Previsão de temperatura: Valores previstos de temperatura, por hora, para duas semanas após o fim da nossa série real.
* Indicadores para alertas: Sempre que a previsão indicar indicar valores 30% superiores a média móvel dos últimos 7 dias, o visual irá indicar um alerta.
* Indicadores para falhas: Sempre que o a temperatura ultrapassar os 90 graus Célsius, teremos uma indicação de falha.
* Filtros: É possível filtrar apenas as válvulas para os quais a previsao indica alerta, selecionar a bivalvula ou face específicas e escolher um período de tempo específico.

Obs: Atualmente contamos com uma câmera térmica na sala de válvulas, logo, está sendo monitorada apenas uma biválvula e uma face.


Detalhes
--------

.. figure:: detalhes.png
    :align: center
    :alt: Aba Detalhes
    :scale: 50%

As funcionalidades presentes na aba "Detalhes" são:

* Série histórica de temperatura: É possível ver a série de valores reais de temperatura, considerando uma válvula por vez.
* Outras séries históricas relevantes: Séries históricas que são correlacionadas com a temperatura das válvulas, como potência ativa e reativa, corrente, temperatura do óleo, entre outras.
* Feature importance: Ranking de importância das demais variáveis ao serem utilizadas para explicar a temperatura das válvulas.
* Estatísticas descritivas: Estatísticas que analisam a correlação entre temperatura e as demais variáveis assim como estatísticas univariadas.
* Métricas de avaliação do modelo: Métricas que avaliam a acurácia do modelo de previsao de temperatura.
* Filtros: Filtro por componente, por período de tempo e por variável a ser comparada com a temperatura.