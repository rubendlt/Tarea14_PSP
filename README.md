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
