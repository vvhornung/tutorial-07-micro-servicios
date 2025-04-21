## A. Creación de template y lanzamiento de nueva instancia en AWS

1,2,3 acceso a curso en aws
![{839D36C1-3A8C-4C6F-B2BA-AE870D5A2D41}](https://github.com/user-attachments/assets/acec8b44-92d3-4544-a31b-636f1aaf9f5e)

4. Ir a la sección de “Modules”.
![{E2AD4259-B0DF-40A5-9A36-949281DED036}](https://github.com/user-attachments/assets/5c22924c-26e4-4e43-ac73-9388303c09c3)

5. Hacer clic en “Launch AWS Academy Learner Lab”.
6. Iniciar el laboratorio haciendo clic en “Start Lab”.
![{3A206B32-BD18-4011-91A5-A5AAD7F501A6}](https://github.com/user-attachments/assets/828ace20-cd33-4739-8dd0-d87f63a48037)

7. Esperar a que el icono de AWS se ponga verde y hacer clic en él.
![{D436E0D0-EC27-47B1-A791-C77944F4738D}](https://github.com/user-attachments/assets/151ccb80-7524-4652-a1ea-307b7296301b)

8. Buscar y seleccionar “EC2”.
![{041FFC61-B467-4086-BBDE-A589DEF64E9F}](https://github.com/user-attachments/assets/0edde3a5-9610-48df-983b-855b1c4b7a25)

9. Ir a “Plantillas de Lanzamiento”.
![{EFF81FBC-B0A8-4944-9881-A3F199D3939C}](https://github.com/user-attachments/assets/d0eb59a7-928e-4f4b-bd52-fed05c65b428)

10. Crear una nueva plantilla de lanzamiento.
![{DB721751-AF9F-4057-8CC9-19533066234D}](https://github.com/user-attachments/assets/2c98d086-ae20-4560-ace1-a0fed2a83a03)

11. Asignar un nombre a la plantilla.
![{64D73A33-CC3E-499C-A946-6D56CF22064D}](https://github.com/user-attachments/assets/59e77961-c97e-4482-a363-0b9793f6b589)

12. Configurar:
    - Amazon Linux como sistema operativo.
    - Tipo de instancia: t2.micro.
    - No incluir par de claves.
    - Crear grupo de seguridad.
      ![{FA25E344-301A-4AE8-BF53-B56408C4FBFF}](https://github.com/user-attachments/assets/3ed8ac33-c5b6-4736-be53-f7cec55ab6d6)
      ![{E757EF8A-D55F-48B5-AA00-FC64936C275B}](https://github.com/user-attachments/assets/1251ac6c-73e9-4225-b58d-f750b8545cdb)
      ![{7C57AAB4-794F-4791-9B8E-07AC789CF661}](https://github.com/user-attachments/assets/6f2c013b-d6c9-4ab3-a185-54f4ab51ce36)



13. Agregar reglas de seguridad e incluir script en "Datos de usuario".
![image](https://github.com/user-attachments/assets/cf049d40-53c0-44a7-a829-213df83e97bb)
![{A2B93A55-B189-4157-A291-44783686E094}](https://github.com/user-attachments/assets/297b88e7-5185-42ed-a11b-4e1f7b8e33e4)


15. Lanzar la instancia desde la plantilla creada.
![{4964DA11-9365-4665-B471-BCA392CB7867}](https://github.com/user-attachments/assets/fb7d3656-f041-43f7-b33a-58b3ca1b2304)

16. Verificar la información.
17. Establecer número de instancias y lanzarlas (sin claves si se solicita).
![{525D6DE6-C51E-4817-AD9B-BD487379BD8D}](https://github.com/user-attachments/assets/6c11d265-e411-465f-b57f-1281e9d1c534)


verificacion de instancia
![{9C4CF2F0-7C4C-4830-A356-3A6EA3F510EA}](https://github.com/user-attachments/assets/30e56817-0203-4490-98f8-eaab9ad2a203)

---

## Inicialización de Docker Swarm

1. Identificar las instancias como `nodo-01` y `nodo-02`.
![image](https://github.com/user-attachments/assets/252d8dba-4ae5-4347-8be6-0678fd43abd0)

2. Conectarse a `nodo-01`.
3. Iniciar Docker Swarm.
![{6C519F5C-3546-40EC-B1F2-FD24C9CBD54E}](https://github.com/user-attachments/assets/91141c0b-e3c7-42ca-abea-cd00b131a893)

4. Generar el token de unión.
sudo docker swarm join --token SWMTKN-1-0j6l0jcss3ir4ud1i9tm8a33a0mfto43qgqzauds2pgu5qbb4a-d4l1wrn56irg0y4fi1t73fesj 172.31.91.191:2377
![{CA37463B-388C-403F-A49B-C63C14096893}](https://github.com/user-attachments/assets/f261cfbb-bfb9-441d-a674-8d925c7c6945)

5. Verificar el nodo activo.
![{C98275FE-4485-43C2-979E-924B30AFC445}](https://github.com/user-attachments/assets/3ceb5128-448d-49e3-b781-c5f0c3c8a879)

---

## B. Conectando nodos al cluster Docker Swarm

1. Conectarse a `nodo-02`.
2. Ejecutar el comando con el token para unirse como manager.
![{AAC7B13D-F49C-4EDF-AF31-1C9EBC876D10}](https://github.com/user-attachments/assets/d5a9e94e-954b-4ca2-83ba-5d732bb22afa)

3. Verificar desde `nodo-01` (o `nodo-02`) que ambos nodos estén conectados.
![{883636AD-689D-45BB-B41E-41A80D8885C7}](https://github.com/user-attachments/assets/7ad3871f-5857-40b0-b571-e545d120abd9)

---

## C. Modificando el proyecto `randomquotes`

1. Modificar el archivo `index.js`.
2. Subir los cambios a GitHub (crear repositorio si no existe).
   ![{74605C58-09D7-43F7-9D23-03EDDC1B077F}](https://github.com/user-attachments/assets/396c5c86-60f7-4550-94d1-086ef73bbc77)
   ![{2A30766D-0BF3-4F85-BD47-B4E2147B66D3}](https://github.com/user-attachments/assets/06c39386-7098-411f-a58d-1664f44063e5)

---

## D. Desplegando el proyecto `randomquotes` en DockerHub

1. Crear cuenta en [dockerhub.com](https://dockerhub.com) y nuevo repositorio.
![{72964074-7AD7-4F41-9F03-7536A1FED743}](https://github.com/user-attachments/assets/9ab2e92c-16b5-4e51-9078-99d7907a249a)


2. Ir al repositorio en GitHub > “Settings” > “Secrets” > “Actions”.

![image](https://github.com/user-attachments/assets/9686e053-5f27-42fd-91e6-01c770dff99f)

3. Agregar los siguientes secretos:
    - `DOCKERHUB_USER`
    - `DOCKERHUB_PASS`

![{16792245-E26B-42C2-BF13-3B22CEC54F04}](https://github.com/user-attachments/assets/69d5fb47-76c6-4937-b7d4-17ec4a19bb4c)

![{B01E38AE-E825-497B-B7C8-173E812E17C5}](https://github.com/user-attachments/assets/38b8576c-aac3-4202-9b3e-7ec1f129a876)

4. Ir a “Actions” y configurar workflow sugerido.
5. Reemplazar configuración por workflow personalizado.
6. Confirmar el commit y verificar ejecución exitosa.

![{80F4F66C-A965-4313-9FC3-02DD291B91B6}](https://github.com/user-attachments/assets/2e3ce6f0-64ce-41a7-8fa9-8fa62d8820bc)

![{C03630A2-BAE9-43AB-92E8-D471245B83B7}](https://github.com/user-attachments/assets/496afab1-b4f1-4f56-a498-2fc541503ff6)


---

## E. Desplegando el proyecto con Docker Service

1. Conectarse a `nodo-01`.
2. Verificar servicios activos.

![{B0F04C21-3832-47AF-9474-71D7AD88F93C}](https://github.com/user-attachments/assets/f846195e-f401-485e-9766-58e683ae2f84)

3. Crear el servicio `randomquotes` con 4 réplicas usando tu imagen de DockerHub.
sudo docker service create --name randomquotes --replicas 4 -p 80:80 vvhornung/express-randomquotes
![{70FDA44C-7BAE-4C96-BB54-7C3B2584B60D}](https://github.com/user-attachments/assets/841aea95-fcc3-4345-b00b-18a98543b346)

4. Ver en qué nodos están las réplicas.
![{5D7A3BAF-8849-4774-9BDA-8975BD5BAA85}](https://github.com/user-attachments/assets/81819351-fe9c-4839-8233-3436d1d37a13)

6. Verificar contenedores en ambos nodos.
![{6408500C-8E1B-4A90-B15A-E03F0B3332A5}](https://github.com/user-attachments/assets/be4c1bb4-c3f3-4a3a-bc54-7de0569bb3bd)
![{40CEAAFF-9959-4661-A3F8-5E7DAA3F921D}](https://github.com/user-attachments/assets/806b8b6a-6703-4aa6-8ea0-d43886d028b1)

7. Acceder a la app desde la IP pública de cualquier nodo.
![{EF951C41-48C3-4B22-AA66-BD38D009D97D}](https://github.com/user-attachments/assets/fdc1d3d4-a860-4774-adc3-b6904c0536f9)
![{2213D197-A762-45A4-9196-E34CCB1EF9E7}](https://github.com/user-attachments/assets/eecca3b0-ed04-44bc-8926-1d79e2a4ce9e)

Felicidades! ¡Ya tienes tus microservicioes corriendo con Docker en la nube! sin pagar ;)

