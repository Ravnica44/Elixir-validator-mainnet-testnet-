Source: https://docs.elixir.xyz/running-an-elixir-validator

SOFTWARE VERSION: 3.5.9 :

MAINNET

`docker rm -f elixir-mainnet`

`docker pull elixirprotocol/validator`

`docker run -d --name elixir-mainnet --env-file validator.env --env ENV=prod --platform linux/amd64 -p 17691:17690 --restart always elixirprotocol/validator`

`docker logs -fn 25 elixir-mainnet`


TESTNET

`docker rm -f elixir`

`docker pull elixirprotocol/validator:testnet`

`docker run -d --name elixir-testnet --env-file validator.env --env ENV=prod --platform linux/amd64 -p 17690:17690 --restart always elixirprotocol/validator:testnet`

`docker logs -f2 25 elixir-testnet`
