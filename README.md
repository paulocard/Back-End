import requests
api_key = "62519aa569b34555bef131202260204"
link_api = "http://api.weatherapi.com/v1/current.json"
parametros= {
    "key" : api_key,
    "q" :"São Paulo",
    "lang" : "pt"
}
resposta = requests.get(link_api, params=parametros)
print(resposta.status_code)
