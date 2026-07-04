{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": []
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
      "cell_type": "code",
      "execution_count": 3,
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "JQCsdk-4G5w2",
        "outputId": "f18c2a79-aa9a-4154-8872-a02a8d81564d"
      },
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "enter:hello\n",
            "olleh\n"
          ]
        }
      ],
      "source": [
        "#Reverse a string\n",
        "stri = str(input(\"enter:\"))\n",
        "stri2 = stri[::-1]\n",
        "print(stri2)"
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Check if a number is prime\n",
        "import math\n",
        "num = int(input(\"enter:\"))\n",
        "if num <= 1:\n",
        "    print(\"not prime\")\n",
        "else:\n",
        "    for i in range(2,int(math.sqrt(num)) + 1):\n",
        "        if num % i == 0:\n",
        "          print(\"not prime\")\n",
        "          break\n",
        "    else:\n",
        "        print(\"prime\")\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Ar5jlEnHH0o5",
        "outputId": "f4768a6f-7626-4121-ea31-8a6d4bfcf605"
      },
      "execution_count": 2,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "enter:66\n",
            "not prime\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Find the second largest number in a list\n",
        "nums = [10,20,30,40,50]\n",
        "\n",
        "largest = second = -9999\n",
        "\n",
        "for num in nums :\n",
        "  if num > largest:\n",
        "    second = largest\n",
        "    largest = num\n",
        "  elif largest > num > second:\n",
        "    second = num\n",
        "print (second)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "f7FFqEAENTwb",
        "outputId": "35afb561-09ca-44f1-93cf-baa5daf2b9d1"
      },
      "execution_count": 6,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "40\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Count vowels in a string\n",
        "stri = str(input(\"enter:\"))\n",
        "\n",
        "count = 0\n",
        "for ch in stri:\n",
        "  if ch in \"aeiouAEIOU\":\n",
        "    count+=1\n",
        "print(count)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "qhzIQD-7PtNk",
        "outputId": "214192e9-91e2-45e1-edb3-65287ecf1286"
      },
      "execution_count": 10,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "enter:Abhinav\n",
            "3\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Fibonacci series\n",
        "n = int(input(\"Enter:\"))\n",
        "\n",
        "a=0\n",
        "b=1\n",
        "\n",
        "for i in range(n):\n",
        "  print(a,end=\" \")\n",
        "  c = a+b\n",
        "  a = b\n",
        "  b = c"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "5KvB-puBQN7_",
        "outputId": "dfc8ef6d-2529-48c2-a9ab-a6c85b8611b3"
      },
      "execution_count": 12,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter:7\n",
            "0 1 1 2 3 5 8 "
          ]
        }
      ]
    }
  ]
}
