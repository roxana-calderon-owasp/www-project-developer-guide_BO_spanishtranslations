---

title: Foundations
layout: col-document
tags: OWASP Developer Guide
contributors: Jon Gadsden
document: OWASP Developer Guide
order: 400
permalink: /draft/foundations/

---

{% include breadcrumb.html %}

<style type="text/css">
.image-right {
  height: 180px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  float: right;
}
</style>

![Developer guide logo](../../assets/images/dg_logo.png "OWASP Developer Guide"){: .image-right }

## 2. Fundamentos

Existen varios conceptos y terminología fundamentales que se utilizan comúnmente en seguridad de software.
Aunque muchos de estos conceptos son complejos de implementar y se basan en una teoría muy estricta,
Los principios suelen ser bastante sencillos y accesibles para todos los ingenieros de software.

Una comprensión razonable de estos conceptos fundamentales permite a los equipos de desarrollo comprender e implementar
Seguridad de software para la aplicación o sistema en desarrollo.
Esta Guía para desarrolladores solo puede brindar una breve descripción general de estos conceptos.
para obtener conocimientos más profundos, consulte los numerosos textos sobre seguridad, como [El conjunto de conocimientos sobre seguridad cibernética] [cbok].

Secciones:

2.1 [Fundamentos de seguridad](01-security-fundamentals.md)  
2.2 [Desarrollo e integración seguros](02-secure-development.md)  
2.3 [Principios de seguridad](03-security-principles.md)  
2.4 [Principios de criptografía](04-crypto-principles.md)  
2.5 [Top 10 de OWASP](05-top-ten.md)  

----

La Guía para desarrolladores de OWASP es un esfuerzo comunitario; si hay algo que necesita cambio
entonces [cree un issue][issue0400] o [edítelo en GitHub][edit0400]

[cbok]: https://www.cybok.org/
[edit0400]: https://github.com/OWASP/www-project-developer-guide/blob/main/draft/04-foundations/toc.md
[issue0400]: https://github.com/OWASP/www-project-developer-guide/issues/new?labels=enhancement&template=request.md&title=Update:%2004-foundations/00-toc