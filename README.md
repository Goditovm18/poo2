[Uploa{
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
      "execution_count": null,
      "metadata": {
        "id": "JhNtNc28WB38"
      },
      "outputs": [],
      "source": [
        "import math\n",
        "\n",
        "class Figura:\n",
        "    def __init__(self, nombre):\n",
        "        self.nombre = nombre\n",
        "        self.area = None\n",
        "        self.perimetro = None\n",
        "\n",
        "    def calcular_area(self):\n",
        "        pass\n",
        "\n",
        "    def calcular_perimetro(self):\n",
        "        pass\n",
        "\n",
        "    def mostrarInfo(self):\n",
        "        self.calcular_area()\n",
        "        self.calcular_perimetro()\n",
        "        print(f\"Nombre de la figura: {self.nombre}\")\n",
        "        print(f\"Área de la figura: {self.area}\")\n",
        "        print(f\"Perímetro de la figura: {self.perimetro}\")\n",
        "\n",
        "class Circulo(Figura):\n",
        "    def __init__(self, nombre, radio):\n",
        "        super().__init__(nombre)\n",
        "        self.radio = radio\n",
        "\n",
        "    def calcular_area(self):\n",
        "        self.area = math.pi * self.radio ** 2\n",
        "\n",
        "    def calcular_perimetro(self):\n",
        "        self.perimetro = 2 * math.pi * self.radio\n",
        "\n",
        "class Cuadrado(Figura):\n",
        "    def __init__(self, nombre, lado):\n",
        "        super().__init__(nombre)\n",
        "        self.lado = lado\n",
        "\n",
        "    def calcular_area(self):\n",
        "        self.area = self.lado ** 2\n",
        "\n",
        "    def calcular_perimetro(self):\n",
        "        self.perimetro = 4 * self.lado\n",
        "\n",
        "class Rectangulo(Figura):\n",
        "    def __init__(self, nombre, base, altura):\n",
        "        super().__init__(nombre)\n",
        "        self.base = base\n",
        "        self.altura = altura\n",
        "\n",
        "    def calcular_area(self):\n",
        "        self.area = self.base * self.altura\n",
        "\n",
        "    def calcular_perimetro(self):\n",
        "        self.perimetro = 2 * (self.base + self.altura)\n",
        "\n",
        "class Triangulo(Figura):\n",
        "    def __init__(self, nombre, base, altura, lado1, lado2, lado3):\n",
        "        super().__init__(nombre)\n",
        "        self.base = base\n",
        "        self.altura = altura\n",
        "        self.lado1 = lado1\n",
        "        self.lado2 = lado2\n",
        "        self.lado3 = lado3\n",
        "\n",
        "    def calcular_area(self):\n",
        "        self.area = (self.base * self.altura) / 2\n",
        "\n",
        "    def calcular_perimetro(self):\n",
        "        self.perimetro = self.lado1 + self.lado2 + self.lado3"
      ]
    }
  ]
}ding Figuras.ipynb…]()
