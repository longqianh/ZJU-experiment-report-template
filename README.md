# ZJU-experiment-report-template

<img src="https://tva1.sinaimg.cn/large/008i3skNly1grjf6dpfpwj30u00v3dnd.jpg" alt="image-20210616003225050" style="zoom: 50%;" />

An experiment report template with LaTeX.

- Compile : XeLaTeX
- Language : 中文
- University : ZJU
- Auther : Peter_H
- Blog : [longqianh.com](https://longqianh.com)



### Tools

- Nice Latex Generators: 

  - [Tables](https://www.tablesgenerator.com/)

  - Formulas : Mathpix Snip

  - [Graphs](https://csacademy.com/app/graph_editor/)

- Image Batch Reformatting:

  - [imagemagick](https://imagemagick.org): convert image format altogether

    - ```shell
      # for macOS
      brew install imagemagick 
      mogrify -format png *.bmp
      ```
      
    - ```bash
      # Terminal code for converting `bmp` file into `png`
      bash -c 'for image in *.bmp; do convert "$image" "${image%.bmp}.png"; echo “image $image converted to ${image%.bmp}.png ”; done'
      ```

      

  - [Fotor](https://www.fotor.com): cutting and processing image online

- Latex to docx:

  - [pandoc](https://medium.com/@zhelinchen91/how-to-convert-from-latex-to-ms-word-with-pandoc-f2045a762293)

    - ```shell
      pandoc --pdf-engine xelatex template.tex -o output.docx
      ```

      

### Todos:

- [{markdown} environment](https://liam.page/2020/03/30/writing-manuscript-in-Markdown-and-typesetting-with-LaTeX/)
- attach mathpix tool
- easily include svg
- ~~latex to word~~