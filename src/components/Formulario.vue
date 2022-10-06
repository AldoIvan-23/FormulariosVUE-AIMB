<script>
    export default {
        data: () => ({

        }),
        methods :{
            registrarProyecto(){
                console.log("Proyecto registrado...")
            },
        },
    };
</script>

<template>
    <form @submit.prevent="registrarProyecto">
        <div class="mb-3">
          <label class="form-label">Proyecto</label>
          <input type="text" class="form-control" required/>
        </div>

        <div class="mb-3">
          <label class="form-label">Actividad</label>
          <select class="form-select" required>
            <option disabled select value="">Seleccione tipo de actividad ...</option>
            <option value="1">Aplicaciones Web con Vue.js</option>
            <option value="2">Backend Service con Node.js</option>
            <option value="3">App Movil con React Native</option>
          </select>
        </div>

        <div class="mb-3 form-check">
          <input type="checkbox" class="form-check-input" id="exampleCheck1">
          <label class="form-check-label" for="exampleImputPassword">Urgente</label>
        </div>
        <button type="submit" class="btn btn-primary">Guardar</button>
      </form>
</template>