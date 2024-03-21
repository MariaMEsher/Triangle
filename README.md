package ru.stqa.geometrty.figured;

import java.awt.geom.Area;

public class Triangle {

    static void printTriangleArea(double a, double b, double c) {
        var p = (a + b + c) / 2;
        var s = Math.sqrt(p * (p - a) * (p - b) * (p - c));
        System.out.println("Площадь треугольника со сторонами" + "=" + p + " * " + (p - a) + " * " + (p - b) + " * " + (p - c) + " =" + triangleArea(a, b, c));
    }

    private static double triangleArea(double a, double b, double c) {
        return a+b+c/2;
    }
}
