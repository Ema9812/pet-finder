
---

## 🔌 Endpoints de la API

### Autenticación

| Método | Endpoint | Descripción | Auth |
|---|---|---|---|
| `POST` | `/auth/register` | Registrar usuario | ❌ |
| `POST` | `/auth/login` | Iniciar sesión (devuelve JWT) | ❌ |

### Mascotas (Pets)

| Método | Endpoint | Descripción | Auth |
|---|---|---|---|
| `POST` | `/pets` | Crear mascota perdida | ✅ |
| `GET` | `/pets` | Listar todas las mascotas | ❌ |
| `GET` | `/pets/:id` | Ver detalle de una mascota | ❌ |
| `PUT` | `/pets/:id` | Actualizar mascota | ✅ |
| `DELETE` | `/pets/:id` | Eliminar mascota | ✅ |
| `GET` | `/pets/search?lat=...&lng=...&radius=...` | Búsqueda geoespacial | ❌ |

### Avistajes (Reports)

| Método | Endpoint | Descripción | Auth |
|---|---|---|---|
| `POST` | `/reports` | Reportar avistaje (dispara email al dueño) | ❌ |
| `GET` | `/pets/:petId/reports` | Ver avistajes de una mascota | ❌ |

---

## 🚀 Cómo correrlo localmente

### 1. Clonar el repo

```bash
git clone https://github.com/Ema9812/pet-finder.git
cd pet-finder