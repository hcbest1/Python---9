# Python---9

{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyNlegwzzVFx2xHqRkcvkV4R",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/ciellleen/copyright/blob/main/9%EC%B0%A8%EC%8B%9C\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0bCl1aMKnf5e",
        "outputId": "239a334d-1fa6-4ed6-ea74-f0a115b330d8"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            " test\n",
            "~~,test,~~ \n",
            "~test\n"
          ]
        }
      ],
      "source": [
        "a = ' test'\n",
        "b = '~~,test,~~ '\n",
        "c = '~test~'\n",
        "print(a.rstrip())\n",
        "print(b.rstrip('~'))\n",
        "print(c.rstrip('~!'))"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = 'test'\n",
        "b = '~~,test,~~'\n",
        "c = '~test!'\n",
        "print( a.lstrip())\n",
        "print( b.lstrip('~'))\n",
        "print( c.lstrip('~!'))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "vhuIyrvUpKAK",
        "outputId": "08cc5de2-c893-4b09-f28a-be755defd9fc"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "test\n",
            ",test,~~\n",
            "test!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = ' test'\n",
        "b = '~~.test.~~ '\n",
        "c = '~test!'\n",
        "print( a.strip() )\n",
        "print( b.strip('~ ') )\n",
        "print( c.strip('~!') )\n",
        "\n",
        "text = ' Water boils at 100 degrees '\n",
        "print('[' + text.rstrip() + ']')\n",
        "print('[' + text.lstrip() + ']')\n",
        "print('[' + text.strip() + ']')"
      ],
      "metadata": {
        "id": "0OffettbpKC-",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "c25f7698-4988-439a-af15-2d696c030eb0"
      },
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "test\n",
            ".test.\n",
            "test\n",
            "[ Water boils at 100 degrees]\n",
            "[Water boils at 100 degrees ]\n",
            "[Water boils at 100 degrees]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "text = '0000000Water boils at 100 degrees 000'\n",
        "print(text.lstrip('0'))\n",
        "print(text.rstrip('0'))\n",
        "print(text.strip('0'))\n",
        "\n",
        "text = \",,,,,123.....water....pp\"\n",
        "print(text.lstrip(',123.p'))\n",
        "print(text.rstrip(',123.p'))\n",
        "print(text.strip(',123.p'))\n",
        "\n",
        "text = ' Water boils at 100 degrees '\n",
        "print(text.lstrip(' Water'))\n",
        "print(text.rstrip(' degrees '))\n",
        "print(text.strip(' degrees '))\n"
      ],
      "metadata": {
        "id": "O73ceQtQpKFy",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "605f30ad-a39e-411d-9431-ca98bdf6bbee"
      },
      "execution_count": 15,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Water boils at 100 degrees 000\n",
            "0000000Water boils at 100 degrees \n",
            "Water boils at 100 degrees \n",
            "water....pp\n",
            ",,,,,123.....water\n",
            "water\n",
            "boils at 100 degrees \n",
            " Water boils at 100\n",
            "Water boils at 100\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "text = '0000000Water boils at 100 degrees 000'\n",
        "print(text.lstrip('0'))\n",
        "print(text.rstrip('0'))\n",
        "print(text.strip('0'))\n",
        "\n",
        "text = \",,,,,123.....water....pp\"\n",
        "print(text.lstrip(',123.p'))\n",
        "print(text.rstrip(',123.p'))\n",
        "print(text.strip(',123.p'))\n",
        "\n",
        "text = ' Water boils at 100 degrees '\n",
        "print(text.lstrip(' Water'))\n",
        "print(text.rstrip(' degrees '))\n",
        "print(text.strip(' degrees '))\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "6QToE5rfz-Q1",
        "outputId": "24868f9c-6415-4815-d91f-e7a903c586b1"
      },
      "execution_count": 18,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Water boils at 100 degrees 000\n",
            "0000000Water boils at 100 degrees \n",
            "Water boils at 100 degrees \n",
            "water....pp\n",
            ",,,,,123.....water\n",
            "water\n",
            "boils at 100 degrees \n",
            " Water boils at 100\n",
            "Water boils at 100\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "txt = \"  Hz  \"\n",
        "x = txt.isspace()\n",
        "print(x)\n",
        "\n",
        "\n",
        "sentence = input(\"문자열을 입력하시오: \")\n",
        "table = { \"알파벳\" : 0, \"숫자\" : 0, \"빈칸\" : 0 }\n",
        "\n",
        "for i in sentence :\n",
        "    if (i.isalpha()):\n",
        "        table[\"알파벳\"] += 1\n",
        "    elif (i.isdigit()):\n",
        "        table[\"숫자\"] += 1\n",
        "    elif (i.isspace()):\n",
        "        table[\"빈칸\"] += 1\n",
        "print(table)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "3DMop7Gf0nB8",
        "outputId": "9e534deb-ab90-4ed2-9c88-434f19bac3cd"
      },
      "execution_count": 21,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "False\n",
            "문자열을 입력하시오: 파이썬(Python)  문자열 관련 함수 사용법\n",
            "{'알파벳': 19, '숫자': 0, '빈칸': 5}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "s = '가나다라'\n",
        "n = 7\n",
        "\n",
        "answer = ''\n",
        "for i in range(n-len(s)): # 문자열의 앞을 빈 문자열로 채우는 for 문\n",
        "    answer += ' '\n",
        "answer += s"
      ],
      "metadata": {
        "id": "gc6tsqzA1ALx"
      },
      "execution_count": 25,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "s = '가나다라'\n",
        "n = 20\n",
        "\n",
        "print(s.ljust(n)) # 좌측 정렬\n",
        "\n",
        "print(s.center(n)) # 가운데 정렬\n",
        "\n",
        "print(s.rjust(n)) # 우측 정렬"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "sHSnhCd21ADi",
        "outputId": "94beb25d-5fcd-442d-f461-9082a480ad5e"
      },
      "execution_count": 26,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "가나다라                \n",
            "        가나다라        \n",
            "                가나다라\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "s = \"a b c d e f g\"\n",
        "print(f's         : {s}')\n",
        "\n",
        "r = s.split()\n",
        "print(f's.split() : {r}')\n",
        "s = \"aa.bb.cc.dd.ee.ff.gg\"\n",
        "print(f's                : {s}')\n",
        "\n",
        "r0 = s.split()\n",
        "r1 = s.split('.')\n",
        "r2 = s.split(sep='.')\n",
        "print(f\"s.split()        : {r0}\")\n",
        "print(f\"s.split('.')     : {r1}\")\n",
        "print(f\"s.split(sep='.') : {r2}\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Z-7FKzNN0nKa",
        "outputId": "ab029d76-5937-4a12-9056-543612b6edca"
      },
      "execution_count": 27,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "s         : a b c d e f g\n",
            "s.split() : ['a', 'b', 'c', 'd', 'e', 'f', 'g']\n",
            "s                : aa.bb.cc.dd.ee.ff.gg\n",
            "s.split()        : ['aa.bb.cc.dd.ee.ff.gg']\n",
            "s.split('.')     : ['aa', 'bb', 'cc', 'dd', 'ee', 'ff', 'gg']\n",
            "s.split(sep='.') : ['aa', 'bb', 'cc', 'dd', 'ee', 'ff', 'gg']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "s = \"aa.bb.cc.BlockDMask.ee.ff.gg.python.example\"\n",
        "print(f'{s}')\n",
        "\n",
        "r0 = s.split()\n",
        "r1 = s.split('.', 3)\n",
        "r2 = s.split(sep='.', maxsplit=3)\n",
        "r3 = s.split('.', maxsplit=3)\n",
        "print(f\"\\ns.split()\\n{r0}\")\n",
        "print(f\"\\ns.split('.', 3)\\n{r1}\")\n",
        "print(f\"\\ns.split(sep='.', maxsplit=3)\\n{r2}\")\n",
        "print(f\"\\ns.split('.', maxsplit=3)\\n{r3}\")\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "4F0kLGNL3viP",
        "outputId": "e23f3900-a2ec-48a5-9d98-6f366ff594b2"
      },
      "execution_count": 28,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "aa.bb.cc.BlockDMask.ee.ff.gg.python.example\n",
            "\n",
            "s.split()\n",
            "['aa.bb.cc.BlockDMask.ee.ff.gg.python.example']\n",
            "\n",
            "s.split('.', 3)\n",
            "['aa', 'bb', 'cc', 'BlockDMask.ee.ff.gg.python.example']\n",
            "\n",
            "s.split(sep='.', maxsplit=3)\n",
            "['aa', 'bb', 'cc', 'BlockDMask.ee.ff.gg.python.example']\n",
            "\n",
            "s.split('.', maxsplit=3)\n",
            "['aa', 'bb', 'cc', 'BlockDMask.ee.ff.gg.python.example']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "txt = \"홈짱닷컴\\nHomzzang.com\"\n",
        "\n",
        "x = txt.splitlines()\n",
        "\n",
        "print(x)\n",
        "g = 'Milk\\nChicken\\r\\nBread\\rButter'\n",
        "\n",
        "print(g.splitlines())\n",
        "print(g.splitlines(True))\n",
        "\n",
        "g = 'Milk Chicken Bread Butter'\n",
        "print(g.splitlines())\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "RM68njS80nPa",
        "outputId": "b382c28e-e7f8-4f9d-9afa-a5db2798d102"
      },
      "execution_count": 29,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "['홈짱닷컴', 'Homzzang.com']\n",
            "['Milk', 'Chicken', 'Bread', 'Butter']\n",
            "['Milk\\n', 'Chicken\\r\\n', 'Bread\\r', 'Butter']\n",
            "['Milk Chicken Bread Butter']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "text = '123,456,789,999'\n",
        "\n",
        "replaceAll= text.replace(\",\",\"\")\n",
        "replace_t1 = text.replace(\",\", \"\",1)\n",
        "replace_t2 = text.replace(\",\", \"\",2)\n",
        "replace_t3 = text.replace(\",\", \"\",3)\n",
        "print(\"결과 :\")\n",
        "print(replaceAll)\n",
        "print(replace_t1)\n",
        "print(replace_t2)\n",
        "print(replace_t3)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "k_sZAXPL4dkz",
        "outputId": "06a96723-d27a-4a4f-f6a6-e97bbcd69bc5"
      },
      "execution_count": 30,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "결과 :\n",
            "123456789999\n",
            "123456,789,999\n",
            "123456789,999\n",
            "123456789999\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = ['a', 'b', 'c', 'd', '1', '2', '3']\n",
        "print(a)\n",
        "print()\n",
        "\n",
        "# 리스트를 문자열로 : join 이용\n",
        "result1 = \"\".join(a)\n",
        "print(result1)\n",
        "\n",
        "\n",
        "# 리스트를 문자열로 : 하나하나 문자열을 더해서.\n",
        "result2 = ''\n",
        "for v in a:\n",
        "    result2 += v\n",
        "\n",
        "print(result2)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "NnkL56VM46EK",
        "outputId": "bb871148-8574-4890-ea49-ec67f0d2d72b"
      },
      "execution_count": 31,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "['a', 'b', 'c', 'd', '1', '2', '3']\n",
            "\n",
            "abcd123\n",
            "abcd123\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "print( \"3\".zfill(3) )\n",
        "\n",
        "print( \"s\".zfill(4) )\n",
        "\n",
        "\n",
        "for x in range(3):\n",
        "    print( str(x).zfill(4) )\n",
        "\n",
        "\n",
        "str = '1234'\n",
        "str_zero = str.zfill(8)\n",
        "print(str_zero)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "UY0iV7ss46GL",
        "outputId": "8b958383-ac5c-46f2-85d9-fd67af84124a"
      },
      "execution_count": 32,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "003\n",
            "000s\n",
            "0000\n",
            "0001\n",
            "0002\n",
            "00001234\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "a = \"abc\"\n",
        "print(a.rjust(10))\n",
        "print(a.rjust(10, '#'))\n",
        "\n",
        "b = \"def\"\n",
        "print(b.ljust(15))\n",
        "print(b.ljust(15, 'k'))"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "z4VhUl5a46Ir",
        "outputId": "139fd9d5-7da3-47ea-9483-e8b2384bcb39"
      },
      "execution_count": 35,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "       abc\n",
            "#######abc\n",
            "def            \n",
            "defkkkkkkkkkkkk\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [],
      "metadata": {
        "id": "z-DiiEA_46LH"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [],
      "metadata": {
        "id": "LxnY5U3O46NM"
      },
      "execution_count": null,
      "outputs": []
    }
  ]
}
