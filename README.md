# Processamento de Imagens

O processamento de imagens foi um projeto de autoria da instrutora [Karina Tiemi Kato](https://www.linkedin.com/in/karina-kato-4b2a56182/), visando a execução prática na criação/geração de pacotes e publicação no Pypi, ministrado na aula **Descomplicando a criação de pacotes de processamento de imagens em Python** , como atividade de entrega do projeto.

> Nota Importante sobre os direitos autorais do Projeto: Os fontes aqui utilizados, são de autoria da instrutora do curso, não sendo o foco da publicação, mas, sim, a utilização dos mesmos, apenas para a criação de pacotes, visto que não possuía os objetos para tal finalidade. Reforço que a utilização aqui, foi somente para a explicação da criação de pacotes. 

### Instituição de Ensino
- [Digital Innovation One](http://www.dio.me/)

---
# Informações do pacote
![Badge](https://img.shields.io/static/v1?label=Versão&message=0.0.1&color=blue&style=plastic)

Funcionalidades do pacote **image_processing-test**:

**Módulo Processing**:
  * Correspondência de histograma;
  * Similaridade estrutural;
  * Redimensionar imagem;

  
**Módulo Utils**:

  * Ler imagem;
  * Salvar imagem;
  * Plotar imagem;
  * Resultado do gráfico;
  * Plotar histograma;

# Upload/Instalação para no Test Pypi
### Passos para hospedar o pacote Python no [Pypi](https://test.pypi.org/)
- [x] Última versão dos pacotes "setuptools" e "wheel"

   ```py -m pip install --user --upgrade setuptools wheel ```

- [x] No próximo passo, certifique-se que o diretório no terminal seja o mesmo onde se localiza o arquivo "setup.py"

   ```C:\SeuDiretorio> py setup.py sdist bdist_wheel```

- [x] Após completar a instalação, verifique se as pastas abaixo foram adicionadas ao projeto:

  - [ ] build;
  - [ ] dist;
  - [ ] image_processing_test.egg-info.


- [x] Após o item anterior, subir os arquivos usando o [Twine](https://pypi.org/project/twine/), para o Test Pypi:

   ```py -m twine upload --repository testpypi dist/*```

- [x] Após a execução do passo anterior no terminal, será pedido para inserir o usuário e senha.
- [x] Dessa forma, o projeto estará hospedado no Test Pypi diretamente.

--- 


# Instalação do pacote localmente, após upload do passo anterior

Instalação local, após hospedagem no Test Pypi

- [x] Instalação das dependências

   ```pip install -r requirements.txt ```

- [x] Instalção do Pacote

Utilize o gerenciador de pacotes ```pip install -i https://test.pypi.org/simple/image-processing-test``` para instalar image_processing-test

   ```pip install image-processing-test```

--- 

# Importação do pacote nos projetos

Comando de importação:

   ```from image-processing-test.processing import combination```
   
Utilização:

   ```combination.find_difference(image1, image2)```

--- 

# Autor 

[Paulo Trevisolli](https://www.linkedin.com/in/trevisolli)

--- 

# Licença

[![Badge](https://img.shields.io/static/v1?label=MIT&message=License&color=green&style=plastic)](https://choosealicense.com/licenses/mit/)

