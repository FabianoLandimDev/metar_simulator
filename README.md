# METAR Trainer — GitHub Pages

Versão 100% estática do METAR Trainer. Não utiliza Flask, Python, backend, banco de dados ou API externa.

## Publicar no GitHub Pages

1. Crie/abra um repositório no GitHub.
2. Coloque **index.html**, **app.js** e **index.css** na pasta que será publicada.
3. Faça commit e push.
4. No repositório, abra **Settings → Pages**.
5. Em **Build and deployment**, selecione **Deploy from a branch**.
6. Escolha a branch (normalmente `main`) e a pasta `/ (root)`.
7. Salve e aguarde a publicação.

O arquivo `index.html` deve estar exatamente na raiz da pasta publicada. Não é necessário `requirements.txt`, `app.py` ou pasta `templates`.

## Uso local

Pode abrir `index.html` diretamente no navegador. Para uma experiência local via servidor estático, use:

```bash
python3 -m http.server 8000
```

e acesse `http://127.0.0.1:8000`.

## Recursos

- geração randômica local de cenários;
- METAR regular sempre em hora cheia;
- SPECI no mesmo aeródromo e fora da hora cheia;
- rosa dos ventos dinâmica;
- vento, rajada e variação;
- visibilidade, tempo presente e obscurecimento;
- temperatura, ponto de orvalho, QNH/QFE/QNE;
- até 3 camadas de nuvens com gênero, oitavos e altura em metros;
- conversão didática para pés e seleção de camadas na correção;
- limite didático de correção das nuvens: <= 3.000 m e <= 9.999 ft;
- correção e pontuação executadas inteiramente no navegador.

> Nota: esta é uma ferramenta didática. Para treinamento operacional formal, utilize sempre a documentação oficial vigente do DECEA/ICEA.
