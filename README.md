# TkrDemo

This is a demo for an OO parser and generater that parses a syntax language and generates QT-based GUI. The parser reads in the language in python comments and generates an AST. Based on the AST, the genearter recursively builds layouts holding different widgets. 


## Example

Syntax langeuage:

```python
"""
PROGRAM test "Hello" OPTION
    FUNCTION function1 one
        HELP
        This is the place for help.
        Help can have several lines.
        END HELP
        PROPERTY MODAL false
        VBOX
            VAR variable1 "String" STRING
                DESC this is a string
                DEFAULT Default
            END VAR
            VAR variable2 "Integer" INTEGER
                DESC this is an integer
                DEFAULT 1
            END VAR
            VAR variable3 "Float" float
                DESC this is a float
                DEFAULT 0.1
            END VAR
            VAR variable4 "Dropdown" library
                DESC this is a library
            END VAR
            VAR variable7 "Boolean" boolean
                DESC this is a boolean
                DEFAULT test_yes test_no
            END VAR
            VAR variable8 "File" file
                DESC this is a file
                DEFAULT xxx.txt
            END VAR
            VAR variable9 "Directory" directory
                DESC this is a directory
                DEFAULT X:/xxx/xxx/xxx
            END VAR
            VAR variable10 "Layer" Layer
                DESC this is a Layer
                choices all
            END VAR
            VAR variable11 "Combo" combo
                DESC this is a combo
                CHOICES TEST_A TEST_B TEST_C TEST_D TEST-E
                DEFAULT TEST_D
            END VAR
            VAR variable13 "Default" default
                DESC this is a default
                DEFAULT Default
            END VAR
        END VBOX
    END FUNCTION
END PROGRAM
"""
```

Generated GUI:


<img width="330" height="305" alt="demo" src="https://github.com/user-attachments/assets/c1906fff-f087-49a0-a4f3-5ca157745fcc" />
