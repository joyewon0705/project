# Markdown Basic Syntax Guide


## Heading

- 제목을 추가하려면 **# 제목** 형식으로 작성함.
- 주의 : # 문자와 텍스트 사이에 반드시 공백을 포함할 것.
- 제목 단계(1~6)에 따라 # 문자 개수를 조절함.
    
    입력:

        ## Level 2
        ### Level 3
        #### Level 4

    출력:

    ## Level 2
    ### Level 3
    #### Level 4

- \# 문자 대신에, 텍스트 아랫줄에 두 개 이상의 = 문자 혹은 - 문자를 추가하면 각각 1단계와 2단계 제목을 생성할 수 있음.

    입력:

        Level 1
        =======
        Level 2
        -------

    출력:

    Level 1
    =======
    Level 2
    -------


## Paragraphs

- 빈 줄을 사용하여 단락을 구분함.
- 주의 : 단락이 리스트에 있지 않는 한, 공백이나 탭으로 문단을 들여쓰지 말 것.

    입력:

        First paragraphs

        Second paragraphs

    출력:

    First paragraphs

    Second paragraphs


## Line Breaks

- 줄 바꿈하려면 후행 공백(두 개 이상의 공백)으로 줄을 끝내고 리턴함.
- 거의 모든 Markdown 응용프로그램에서 후행 공백 대신 HTML tag \<br>을 사용할 수 있음.

    입력:

        This is the first line.  
        And this is the second line.

    출력:

    This is the first line.  
    And this is the second line.


## Emphasis

### Bold

- 텍스트를 굵게 표시하려면 텍스트 앞뒤에 ** 또는 __ 를 추가함.
    - 예) \*\*bold text\*\* -> **bold text**
- 단어 중간을 굵게 표시하려면 공백없이 ** 를 추가함.
    - 예) Love\*\*is\*\*bold -> Love**is**bold

### Italic

- 텍스트를 기울이려면 텍스트 앞뒤에 * 문자 또는 _ 문자를 추가함.
    - 예) \*cat's meow\* -> *cat's meow*
- 단어 중간을 기울이려면 공백없이 * 문자를 추가함.
    - 예) A\*cat\*meow -> A*cat*meow

### Bold and Italic

- 텍스트를 굵고 기울여 표시하려면 *** 혹은 ___ 를 추가함.
    - 예) \*\*\*really important\*\*\* -> ***really important***
- 단어 중간을 굵고 기울여 표시하려면 공백없이 *** 를 추가함.
    - 예) really\*\*\*very\*\*\*important -> really***very***important


## Blockquotes

- 단락 앞에 > 문자를 추가해 인용구를 만듦.

    입력:

        > The rendered output looks like this.

    출력:

    > The rendered output looks like this.

- 단락 사이의 빈 줄에 > 문자를 추가해 여러 단락을 포함할 수 있음.

    입력:

        > Blockquote A
        >
        > Blockquote B

    출력:

    > Blockquote A
    >
    > Blockquote B

- 단락 앞에 >> 를 추가해 인용구를 중첩함.

    입력:

        > Blockquote A
        > 
        >> Nested Blockquote

    출력:

    > Blockquote A
    > 
    >> Nested Blockquote

- 인용구는 여러 요소를 포함할 수 있음.

    입력:

        > ### Other Markdown formatted Elements
        >
        > - Not all elements can be used 
        > 
        > you’ll need to __experiment__ to see *which ones work*.

    출력:

    > ### Other Markdown formatted Elements
    >
    > - Not all elements can be used 
    > 
    > you’ll need to __experiment__ to see *which ones work*.


## Lists

### Oredered Lists

- 숫자와 마침표를 추가해 정렬된 리스트 항목을 생성함.

    입력:

        1. First item
        2. Second item

    출력:
    
    1. First item
    2. Second item

- 주의 : 숫자는 1234 순서일 필요는 없지만 반드시 1로 시작해야 함.

    입력:

        1. First item
        1. Second item
        4. Third item

    출력:

    1. First item
    1. Second item
    4. Third item
    
- 중첩된 리스트를 만들려면 하나 이상의 항목을 들여씀.

### Unordered Lists

- \- 문자, * 문자 또는 + 문자를 추가해 정렬되지 않은 리스트 항목을 생성함.

    입력:

        - First item
        - Second item

    출력:

    - First item
    - Second item

- 주의 : 동일한 리스트 내에서는 동일한 구분 기호를 사용해야 함.
- 중첩된 리스트를 만들려면 하나 이상의 항목을 들여씀.

### Adding Elements in Lists

- 리스트의 연속성을 유지하면서 다른 요소(Paragraphs, Blockquotes, Images, Lists)를 추가하려면 공백 4개 또는 탭 1번으로 들여씀.
- Code Blocks은 공백 8개 또는 탭 2번으로 들여씀.


## Code

- 텍스트를 ` 문자로 묶으면 코드로 표시됨.
- 코드로 표시하려는 텍스트에 ` 문자가 포함된 경우엔 단어나 구를 이중으로 묶음.
    - 예) \`\`Use \`code\` in your Markdown file.\`\` -> ``Use `code` in your Markdown file.``
- Code Blocks을 만들려면 해당되는 모든 줄을 최소 4개의 공백 또는 탭 1번으로 들여씀.  

        Code Block looks like this.


## Horizontal Rules

- 가로선을 만들려면  3개 이상의 * 문자, - 문자, 또는 _ 문자를 한 줄에 단독으로 나열함.
- 주의 : 가로선 앞 뒤에 빈 줄을 추가할 것.

    입력:

        ***

    출력:

    ***


## Links

- 링크를 만들려면 **\[연결할 텍스트\]\(URL\)** 형식으로 작성함.
    - 예) \[Duck Duck Go\]\(https://duckduckgo.com\) -> [Duck Duck Go](https://duckduckgo.com)
- 주의 : URL에 공백이 있는 경우 공백 대신 %20을 쓸 것.
- 링크 제목을 추가하려면 따옴표로 묶어 괄호 안, URL 뒤에 추가함.
    - 예) \[Duck Duck Go\]\(https://duckduckgo.com "Title"\) -> [Duck Duck Go](https://duckduckgo.com "Title")
- URL이나 이메일 주소를 <> 로 묶으면 링크로 전환할 수 있음.
- 괄호 앞뒤에 문자를 추가해 링크를 강조하거나 코드로 표시할 수 있음.
    - 예) \*\*\[EFF\]\(https://eff.org\)\*\* -> **[EFF](https://eff.org)**

### Reference-style Links

#### Formatting the First Part of the Link

- **[연결할 텍스트] [레이블]** 형식으로 작성함.
- 레이블은 문서의 다른 곳에 저장된 링크를 가리키는 데 사용됨.
- 레이블은 문자, 숫자, 공백, 구두점을 포함할 수 있음.

#### Formatting the Second Part of the Link

- **[레이블]: URL** 형식으로 작성함.
- URL은 <> 로 묶어도 됨.
- 링크 제목을 추가하려면 따옴표 혹은 괄호로 묶어서 링크 뒤에 추가함.

#### Example
입력:

    it was a [hobbit-hole][1], and that means comfort.

    [1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'

출력:  

it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'


## Image

- 이미지를 추가하려면 **![대체 텍스트](이미지 경로 또는 URL)** 형식으로 작성함.
- 제목을 추가하려면 따옴표로 묶어서 괄호 안 경로 뒤에 추가함.

    입력:  

        ![Philadelphia's Magic Gardens. This place was so cool!](./images/philly-magic-garden.jpg "Philadelphia's Magic Gardens")

    출력:  

    ![Philadelphia's Magic Gardens. This place was so cool!](./images/philly-magic-garden.jpg "Philadelphia's Magic Gardens")

- 이미지에 링크를 추가하려면 **[![대체 텍스트](이미지 경로 또는 URL)](링크 URL)** 형식으로 작성함.

    입력:

        [![An old rock in the desert](./images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

    출력:

    [![An old rock in the desert](./images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)


## Escaping Characters

- Markdown 문서에서 텍스트 서식을 지정하는 데 사용되는 리터럴 문자를 표시하려면 앞에 \ 문자를 추가함.
    - 예) \\\* -> \*
- 가능한 문자 : \\, \`, \*, \_, \{\}, \[\], \<\>, \(\), \#, \+, \-, \., \!, \|


## HTML

- 많은 Markdown 응용 프로그램에서 일부 HTML tag를 사용할 수 있음.
    - 예) This \<em>word\</em> is italic. -> This <em>word</em> is italic.


## +) [GitHub repository URL](https://github.com/joyewon0705/S-W-Engineering.git)