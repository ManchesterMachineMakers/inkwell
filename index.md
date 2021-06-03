---
layout: landing
header:
    title: Inkwell
    slogan: A modern theme for Jekyll sites
    logo: /assets/InkwellLogo.svg
    buttons:
        - title: Get Started
          url: '#get-started'
title: "Home"
---

# Inkwell
Inkwell is a modern theme for Jekyll sites.

## Get Started
To use Inkwell in your site, use the normal GitHub Pages `remote_theme` method:
```yaml
remote_theme: ManchesterMachineMakers/inkwell
```
Some more syntax:
```java
import java.lang.reflect.*;
import java.lang.annotation.*;

public class Basic {
    public static void main(String[] args) {
        // SETUP //
        System.out.println("Hello Java Reflection");

        // GETTING THE NAME OF A CLASS //
        Class<?> cls = Basic.class;
        System.out.println("The class's name is " + cls.getName());
        
        // GETTING THE NAME OF A METHOD //
        Basic basic = new Basic();
        basic.doSomething("whatever");
        try {
            Method doSomething = cls.getMethod("doSomething", String.class);
            System.out.println("The method's name is " + doSomething.getName());
        } catch(NoSuchMethodException e) {
            System.out.println("A whatsit happened: " + e.toString());
        }
    }
    public void doSomething(String whatever) {
        System.out.println("Doing something very interesting...");
        System.out.println("Whatever is " + whatever);
    }
}
```