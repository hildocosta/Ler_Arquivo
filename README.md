<p align="center">
  <img src="https://github.com/hildocosta/hildocosta-Curso-Java--Nelio-Alves/blob/main/logo.png" width="300">
</p>

<h1 align="center">🚀 Explorando Leitura de Arquivo Texto em Java</h1>

<p>🔥 Bem-vindo ao repositório dedicado à exploração da leitura de arquivos de texto na linguagem de programação Java. Aqui, você encontrará informações e exemplos práticos sobre como usar as classes File e Scanner para ler e processar dados de arquivos de texto em seus programas Java.</p>

<p>🎓 Este repositório é voltado para estudantes e desenvolvedores que desejam aprender como ler dados de arquivos de texto de forma eficiente e prática em Java. Aqui, você encontrará explicações detalhadas, exemplos de código e exercícios para aprimorar suas habilidades de leitura de arquivos.</p>

<p>💡 Ao explorar a leitura de arquivos texto em Java, você aprenderá como abrir, ler e processar dados de arquivos de texto usando as classes File e Scanner. Essas classes fornecem métodos simples e eficazes para trabalhar com arquivos de texto, permitindo que você extraia informações de arquivos de forma fácil e rápida.</p>

<h2 align="center">🔒 Licença</h2>

<p>⚖️ Este projeto está licenciado sob a <a href="LICENSE">Licença MIT</a>.</p>

<h2 align="center">📧 Contato</h2>

<h3>🔗 Redes Sociais e Contato</h3>

<ul>
  <li>📌 GitHub: <a href="https://github.com/hildocosta">hildocosta</a></li>
  <li>💼 LinkedIn: <a href="https://www.linkedin.com/in/hildo-costa-b83812231/">Hildo Costa</a></li>
  <li>✉️ Email: hildo.costa@pm.pr.gov.br</li>
</ul>

<p>Agora que estamos preparados, vamos explorar como ler arquivos de texto em Java!</p>

<h2 align="center">🚀 Vamos Começar</h2>

<h3>🔥 Leitura de Arquivo Texto em Java</h3>

<p>Para ler dados de um arquivo de texto em Java, você pode usar as classes File e Scanner. A classe File representa o arquivo em disco, enquanto a classe Scanner é usada para ler os dados do arquivo.</p>

<p>Veja um exemplo de código para ler um arquivo de texto em Java:</p>

```java
import java.io.File;
import java.io.IOException;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        
        File file = new File("caminho/do/arquivo.txt");
        
        try {
            Scanner scanner = new Scanner(file);
            while (scanner.hasNextLine()) {
                System.out.println(scanner.nextLine());
            }
            scanner.close();
        } catch(IOException e) {
            System.out.println("Erro ao ler o arquivo: " + e.getMessage());
        }
    }
}
