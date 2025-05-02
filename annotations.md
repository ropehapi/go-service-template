# Annotations by ropehapi
Para o perfeito funcionamento da aplicação, foi necessário fazer algumas modificações:
- Criar um diretorio temporario para a execução dos testes
- Ajustar o makefile para rodar os testes incluindo esse diretório temporário
- Instalar o staticcheck com:
 `go install honnef.co/go/tools/cmd/staticcheck@latest`
 `export PATH="$PATH:$(go env GOPATH)/bin"`
 `source ~/.bashrc  # ou ~/.zshrc`
- Instalar o govulncheck com:
 `go install golang.org/x/vuln/cmd/govulncheck@latest`
 `export PATH="$PATH:$(go env GOPATH)/bin"`
 `source ~/.bashrc  # ou ~/.zshrc`

*os binários serão instalado no seu $GOBIN, que por padrão é: `$HOME/go/bin`