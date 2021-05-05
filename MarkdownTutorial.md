# Markdown Basic Syntax Guide

main 브랜치에서 작업한 내역 

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


