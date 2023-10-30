Resultados após execução:

parte do codigo usada para fazer a media de pessoas por mes:<br>

  SELECT <br>
  YEAR(dia) AS ano,<br>
  MONTH(dia) AS mes,<br>
  COUNT(*) AS num_pacientes,<br>
  COUNT(DISTINCT id_veiculo) as num_veiculos,<br>
  COUNT(*) / COUNT(DISTINCT id_veiculo) AS media_pacientes_por_veiculo<br>
  FROM <br>
  logistica.trans_pacientes<br>
  GROUP BY<br>
  ano, mes;<br>

  resultado:<br>
  <img src="imagem_resultado.jpg">


Diagrama:<br>
<img src="diagrama.jpg">

<br>
Acesso ao banco de dados:<br>

hostname: http://dbponderada.cc0qa9him3hl.us-east-1.rds.amazonaws.com<br>
nome de usuario: admin<br>
senha para acesso: 12345678
