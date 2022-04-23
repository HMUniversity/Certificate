# Certificate

HM University Certificate


## Usage

1. Fork the repo 
2. Go to `stchi-cert.tex` or `stlinus-cert.tex`
3. Go to this part of the file:

    ``` tex
    \newcommand{\NAME}{YOUR\_NAME\_HERE}
    \newcommand{\YEAR}{YEAR}
    \newcommand{\DATE}{DATE}
    ```

4. Replace `YOUR\_NAME\_HERE` by your name, `YEAR` by the current year and `DATE` by the current date.

    **Do not change the `{\YEAR}` and `{\DATE}` !**

5. Commit and push to `Github`, then open `Github Actions` to download your certificate!

## Compile

1. **Makesure** you have `LaTeX` environment installed!

2. Clone git repository

    ```bash
    git clone https://github.com/HMUniversity/Certificate.git
    ```

3. Open the `tex` file depending to the certification that you want to get, and go to this part of the file:

    ``` tex
    \newcommand{\NAME}{YOUR\_NAME\_HERE}
    \newcommand{\YEAR}{YEAR}
    \newcommand{\DATE}{DATE}
    ```

4. Replace `YOUR\_NAME\_HERE` by your name, `YEAR` by the current year and `DATE` by the current date.

    **Do not change the `{\YEAR}` and `{\DATE}` !**

5. Then run 

    ```bash
    xelatex -synctex=1 -interaction=nonstopmode -file-line-error -pdf stchi-cert.tex 
    ```

    for certificate of St. Chi College, or

    ```bash
    xelatex -synctex=1 -interaction=nonstopmode -file-line-error -pdf stlinus-cert.tex 
    ```

    for certificate of St. Linus College.

6. Get `stchi-cert.pdf` or `stlinus-cert.pdf`!
