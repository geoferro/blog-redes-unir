---
layout: default
title: "Evolución de los protocolos web: De HTTP/1.1 a HTTP/3 sobre QUIC"
date: 2026-10-25 10:00:00 -0500
categories: arquitectura
image: "https://images.unsplash.com/photo-1558494949-ef010cbdcc31?auto=format&fit=crop&w=1000&q=80"
---

<article class="post-full">
    <div class="post-meta">25 de Octubre, 2026 | Arquitectura de Red</div>
    <h1>{{ page.title }}</h1>
    <img src="{{ page.image }}" alt="Infraestructura de servidores de red" class="post-image">
    <p>En el desarrollo de aplicaciones en red modernas, la latencia del protocolo de transporte determina directamente el rendimiento percibido por el usuario final. Durante años, HTTP/1.1 y HTTP/2 operaron sobre TCP, lo que introdujo el problema conocido como <strong>Head-of-Line (HoL) blocking</strong> en la capa de transporte: si un único paquete TCP se pierde en tránsito, todos los flujos multiplexados deben esperar su retransmisión.</p>
    <p>La llegada de <strong>HTTP/3</strong> resuelve este cuello de botella reemplazando TCP por <strong>QUIC</strong>, un protocolo de transporte construido sobre UDP. Al gestionar los flujos de manera independiente e integrar el handshake criptográfico TLS 1.3 dentro del propio establecimiento de conexión (1-RTT e incluso 0-RTT), reducimos drásticamente el tiempo de respuesta en redes móviles e inestables.</p>
    <p><a href="{{ '/' | relative_url }}" class="btn-read">&larr; Volver al índice</a></p>
</article>
