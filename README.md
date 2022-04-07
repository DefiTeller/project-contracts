Репозиторий адресов контрактов и токенов.

Адреса контрактов и токенов хранятся в папке projects.

Чтобы добавить токены нужно в файл projects/tokens.json добавить токен в формате   
 ``` json
[   
    {
        "platforms": {
            "1": "0x08d967bb0134F2d07f7cfb6E246680c53927DD30",
            "56": "0xF218184Af829Cf2b0019F8E6F0b2423498a36983",
            "42161": "0x99F40b01BA9C469193B360f72740E416B17Ac332"
        },
        "name": "MATH",
        "symbol": "math",
        "decimals": 18
    },
]
```

где "1", "56", "42161" в блоке `platforms` это blockchain ID, который можно взять в https://chainlist.org/.


Чтобы добавить адрес контракта нужно папке  projects найти подпапку с соответсвующим именем.
Например для Sushi swap -> 4_sushi.
Добавить  в файле projects/4_sushi/сontracts.json адреса в формате :
```json
{
  "1": [
    "0x00040A7ebfc9F6Fbce4D23bD66b79A603Ba1c323",
    "0x00088E1f7510370fAb86a7bd10578b578C61c723"
  ],
  "56": [
    "0xF218184Af829Cf2b0019F8E6F0b2423498a36983"
  ]

}
```
Где "1", "56" это blockchain ID, который можно взять в https://chainlist.org/.