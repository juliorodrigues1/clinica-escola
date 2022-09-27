<template>
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <v-col cols="12" md="6">
          <v-text-field v-model="firstname" :rules="nameRules" label="Nome Completo" required></v-text-field>
        </v-col>

        <v-col cols="12" md="6">
          <v-text-field v-model="email" :rules="emailRules" label="E-mail" required></v-text-field>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12" md="6">
          <v-radio-group v-model="row" row label="Possui nome social?">
            <v-radio label="sim" value="1"></v-radio>
            <v-radio label="Não" value="0"></v-radio>
          </v-radio-group>

        </v-col>

        <v-col cols="12" md="6">
          <v-text-field v-model="nomeSocial" label="Nome Social"></v-text-field>
        </v-col>


      </v-row>

      <v-row>
        <v-col cols="12" md="6">
          <v-radio-group v-model="row" row label="Gênero:">
            <v-radio label="Feminino" value="feminino"></v-radio>
            <v-radio label="Masculino" value="masculino"></v-radio>
            <v-radio label="Outro" value="outro"></v-radio>
            <v-radio label="prefiro não dizer" value="nao"></v-radio>
          </v-radio-group>
        </v-col>

        <v-col cols="12" md="6">
          <label>Você é</label>
          <v-checkbox v-model="ex4" label="Acadêmico" color="blue" value="1" hide-details></v-checkbox>
          <v-checkbox v-model="ex4" label="Colaborador (Administrativo/Geral)" color="blue" value="2" hide-details>
          </v-checkbox>
          <v-checkbox v-model="ex4" label="Colaborador (Docente)" color="blue" value="3" hide-details></v-checkbox>
        </v-col>
      </v-row>

      <v-row>
        <v-col cols="12" md="6">
          <v-text-field v-model="matricula" label="Se for aluno da U:VERSE, qual seu número de matrícula?">
          </v-text-field>
        </v-col>
      </v-row>

      <v-col cols="12" md="6">
        <v-radio-group v-model="row" row label="Se for acadêmico na U:VERSE, é aluno/a do curso de:">
          <v-col cols="12">
            <v-radio label="Administração" value="Administração"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Análise e Desenvolvimento de Sistema" value="Análise e Desenvolvimento de Sistema">
            </v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Arquitetura e Urbanismo" value="Arquitetura e Urbanismo"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Ciências Contábeis" value="Ciências Contábeis"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Direito" value="Direito"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Engenharia Civil" value="Engenharia Civil"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Gestão de Serviços Jurídicos e Notariais" value="Gestão de Serviços Jurídicos e Notariais">
            </v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Gestão Pública" value="Gestão Pública"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Psicologia" value="Psicologia"></v-radio>
          </v-col>
          <v-col cols="12">
            <v-radio label="Serviço Social" value="Serviço Social"></v-radio>
          </v-col>
        </v-radio-group>
      </v-col>

    </v-container>
  </v-form>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: "FormularioPaciente",
  data: () => ({
    form: {},
    valid: false,
    firstname: '',
    nameRules: [
      v => !!v || 'Nome é obrigatorio',
      v => v.length >= 3 || 'O nome deve ter no monimo 3 caracteres',
    ],
    email: '',
    emailRules: [
      v => !!v || 'E-mail é obrigatorio',
      v => /.+@.+/.test(v) || 'E-mail invalido',
    ],
  }),
})
</script>
