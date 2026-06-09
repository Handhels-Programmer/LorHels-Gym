# LorHels-Gym

### 🏋️‍♂️ Plataforma Integral de Fitness

**Definición Técnica:**
LorHels Gym es una **Aplicación Web de Página Única (SPA - Single Page Application)** construida con una arquitectura *Serverless* (sin servidor tradicional). Utiliza **Vanilla JavaScript** con módulos ES6 para la lógica, **Tailwind CSS** para un diseño responsivo y moderno, y **Firebase** (Authentication y Firestore) como Backend-as-a-Service (BaaS) para la base de datos en tiempo real y la gestión de usuarios.

**Propósito Comercial:**
Es un ecosistema digital diseñado para centralizar la gestión de un gimnasio o servicio de entrenamiento personal. Conecta a administradores, entrenadores profesionales y atletas bajo una misma plataforma, automatizando la entrega de rutinas, el control de pagos y el seguimiento del rendimiento físico.

---

### 👥 Sistema de Roles (RBAC)

La aplicación divide su comportamiento y permisos en tres tipos de cuentas:

1. **🛡️ Administrador (Admin):**
* Tiene el control total del negocio.
* Crea y gestiona los **Planes de Suscripción** (precios, duración, límites de alumnos).
* Aprueba o rechaza los pagos y suscripciones de todos los usuarios.
* Administra la **Biblioteca Global de Ejercicios** (crea nuevos o aprueba los propuestos por los entrenadores).
* Visualiza las métricas generales del gimnasio (Dashboard).


2. **💪 Entrenador Profesional (Trainer):**
* Paga una suscripción para usar la plataforma y gestionar a sus propios clientes.
* Tiene un límite de alumnos basado en el plan que haya comprado (Básico, Élite, Ilimitado, etc.).
* Puede proponer nuevos ejercicios a la biblioteca global.
* Crea, personaliza y asigna **Rutinas** directamente a los perfiles de sus alumnos.
* Monitorea el progreso, la fatiga y el historial de entrenamiento de cada uno de sus clientes.


3. **🏃 Atleta (User):**
* Paga una suscripción para acceder a los servicios de entrenamiento.
* Selecciona a su entrenador personal del catálogo disponible.
* Visualiza sus rutinas asignadas y ejecuta el **Modo Entrenamiento**.
* Registra su peso, altura y el volumen levantado (lbs x reps) en cada sesión.
* Visualiza su evolución a través de gráficas y su mapa de fatiga muscular.



---

### ⭐ Características Estrella (Core Features)

* **Motor de Entrenamiento en Vivo:** Un asistente paso a paso que guía al atleta durante su rutina en el gimnasio, incluyendo temporizadores automáticos de descanso y alertas sonoras.
* **Body Tracker (Mapa de Fatiga Muscular):** Un sistema visual inteligente que lee el historial del usuario de los últimos 7 días y colorea un mapa del cuerpo humano indicando qué músculos están descansados, trabajados o fatigados.
* **Gráficas de Rendimiento:** Integración con `Chart.js` para dibujar la curva de volumen total levantado a lo largo del tiempo.
* **Flujo de Pagos Integrado:** Sistema ágil donde la compra de planes redirige directamente a WhatsApp con un mensaje preformateado para enviar el comprobante de pago al administrador.
