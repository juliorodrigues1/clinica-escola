<template>
  <form>
    <div class="row">
      <div class="col">
        <label class="form-label">Nome:</label>
        <input class="form-control" type="text">
      </div>

      <div class="col">
        <label class="form-label">Email></label>
        <input class="form-control" type="email">
      </div>
    </div>

    <div class="row">
      <div class="col">
        <label for="form-label">Você usa nome social?</label>
        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault1">
          <label class="form-check-label" for="flexRadioDefault1">
            Sim
          </label>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2">
          <label class="form-check-label" for="flexRadioDefault2">
            Não
          </label>
        </div>
      </div>

      <div class="col">
        <label class="form-label">Nome Social:</label>
        <input type="text" class="form-control">
      </div>
    </div>

    <div class="row">
      <div class="col">
        <label class="form-label">Gênero</label>
        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault1">
          <label class="form-check-label">
            Feminino
          </label>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2">
          <label class="form-check-label">
            Masculino
          </label>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2">
          <label class="form-check-label">
            Outro
          </label>
        </div>

        <div class="form-check">
          <input class="form-check-input" type="radio" name="flexRadioDefault" id="flexRadioDefault2">
          <label class="form-check-label">
            Prefiro não dizer
          </label>
        </div>
      </div>

      <div class="col">
        <label class="form-label">Você é?</label>
        <div class="form-check">
          <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault">
          <label class="form-check-label" for="flexCheckDefault">
            Acadêmico
          </label>
        </div>

        <div class="form-check">
          <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault">
          <label class="form-check-label" for="flexCheckDefault">
            Colaborador (Administrativo/Geral)
          </label>
        </div>

        <div class="form-check">
          <input class="form-check-input" type="checkbox" value="" id="flexCheckDefault">
          <label class="form-check-label" for="flexCheckDefault">
            Colaborador (Docente)
          </label>
        </div>
      </div>

    </div>

    <div class="row">
        <div class="col">
          <label class="form-label">Se for aluno da U:VERSE, qual seu número de matrícula?</label>
          <input type="text" class="form-control">
        </div>

        <div class="col">
          
        </div>
      </div>
  </form>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: "FormularioPaciente",
})
</script>
