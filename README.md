# Tarea14_PSP

## Apartado 1

Creamos la tabla con este query
```sql
CREATE TABLE public."EmpresasFCT" (
    idEmpresa SERIAL PRIMARY KEY,
    nombre VARCHAR(40),
    quiereAlumnos BOOLEAN,
    numAlumnos INTEGER,
    fechaContacto DATE
);
```
<img width="1500" height="678" alt="Captura desde 2025-12-01 11-42-52" src="https://github.com/user-attachments/assets/e8a04204-f106-4f87-901e-819b20d71133" />
<img width="287" height="313" alt="Captura desde 2025-12-01 11-46-34" src="https://github.com/user-attachments/assets/629f8ee7-1012-4399-acff-e64be4a4e0de" />

## Apartado 2

Insertamos los datos con este query
```sql
INSERT INTO public."EmpresasFCT" (nombre, quiereAlumnos, numAlumnos, fechaContacto)
VALUES
('Real Madrid', TRUE, 15, '2025-12-01'),
('FC Barcelona', TRUE, 12, '2025-11-25'),
('Atlético de Madrid', FALSE, 0, '2025-12-05'),
('Sevilla FC', TRUE, 8, '2025-11-30'),
('Valencia CF', FALSE, 0, '2025-12-02');
```
<img width="1475" height="728" alt="Captura desde 2025-12-01 11-51-49" src="https://github.com/user-attachments/assets/27528d82-56d1-406c-9265-c359e41e53ce" />
<img width="1570" height="794" alt="Captura desde 2025-12-01 11-54-23" src="https://github.com/user-attachments/assets/5978281b-4076-458b-bb1f-d03840ef5e03" />

## Apartado 3

Hacemos la consulta con este query
```sql
SELECT * FROM public."EmpresasFCT" ORDER BY fechaContacto DESC;
```
<img width="1570" height="794" alt="Captura desde 2025-12-01 12-00-12" src="https://github.com/user-attachments/assets/f488d05c-2fd8-4886-bc8f-1795a975b8a5" />

## Apartado 4

Este es el query
```sql
SELECT rp.name AS "Nombre", rp.city AS "Ciudad", rpe.name AS "Nombre Comercial de la Empresa" 
FROM res_partner rp LEFT JOIN res_partner rpe ON rp.parent_id = rpe.id WHERE rp.parent_id 
IS NOT NULL AND rp.city <> 'Tracy' ORDER BY rpe.name ASC;
```
<img width="1570" height="794" alt="Captura desde 2025-12-01 12-03-04" src="https://github.com/user-attachments/assets/b657fcc2-080e-44e9-a9cf-77f259124a90" />

## Apartado 5

<img width="1570" height="794" alt="Captura desde 2025-12-01 12-07-01" src="https://github.com/user-attachments/assets/e3cc9cc6-c420-436a-8244-cea7bfeed26c" />

## Apartado 6

<img width="1570" height="794" alt="Captura desde 2025-12-01 12-09-09" src="https://github.com/user-attachments/assets/a9b6733a-16b6-4d83-8524-c23c806e16d5" />

## Apartado 7

<img width="1570" height="794" alt="Captura desde 2025-12-01 12-11-14" src="https://github.com/user-attachments/assets/438f112d-7c25-4ab7-b7e5-4cf539d57b33" />
<img width="1570" height="794" alt="Captura desde 2025-12-01 12-11-36" src="https://github.com/user-attachments/assets/2d72e87a-20ae-4f3b-a43a-05fa021fa050" />


