SOFTWARE VERSION: 3.5.9 :

Source: https://docs.elixir.xyz/running-an-elixir-validator

`docker rm -f elixir-mainnet`

`docker pull elixirprotocol/validator`

`docker run -d --name elixir-mainnet --env-file validator.env --env ENV=prod --platform linux/amd64 -p 17691:17690 --restart always elixirprotocol/validator`

`docker logs -f elixir-mainnet`