# Projeto Spring Boot - Hello World

Este repositório contém um projeto Spring Boot simples que expõe um endpoint REST retornando a mensagem "Hello, World!".

## 🚀 Tecnologias Utilizadas
- Java 17+ (ou versão compatível)
- Spring Boot
- Spring Web
- Maven

## 📌 Configuração do Projeto

### 1️⃣ Clonar o Repositório
```bash
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/Arthurhff/ArquiteturaWeb-HelloWord)
cd ArquiteturaWeb-HelloWord
```

### 2️⃣ Construir e Executar a Aplicação
Certifique-se de ter o Java e Maven instalados. Para rodar o projeto, utilize o seguinte comando:
```bash
mvn spring-boot:run
```
A aplicação será iniciada e estará disponível em `http://localhost:8080/api/arthurfonseca`.

## 🔥 Código do Endpoint
A classe `HelloController` implementa um endpoint simples:
```java
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@RestController
@SpringBootApplication

public class DemoApplication {

	public static void main(String[] args) {
		SpringApplication.run(DemoApplication.class, args);
	}

	@GetMapping("/api/arthurfonseca")
	public String hello(){
		return "Hello Word!";
	}
}
```

## 🛠 Testando a API
Após iniciar a aplicação, acesse `http://localhost:8080/api/arthurfonseca` pelo navegador ou via terminal:
```bash
curl -X GET http://localhost:8080/api/arthurfonseca
```
A resposta esperada é:
```bash
Hello World!
```
📌 **Link do Repositório:** [GitHub](https://github.com/Arthurhff/ArquiteturaWeb-HelloWord)


