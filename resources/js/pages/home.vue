<template>
  <card :title="$t('pre-register-status')">
    <table class="table table-bordered">
      <thead>
        <tr>
          <th style="width: 50%">
            {{ $t('name') }}
          </th>
          <th style="width: 10%">
            {{ $t('status') }}
          </th>
          <th style="width: 25%">
            {{ $t('grade_year_level') }}
          </th>
          <th style="iwdth: 15%">
            {{ $t('quick-actions') }}
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Lorem ipsum dolor sit amet consectetur adipisicing elit. Libero maxime cum est?</td>
          <td>
            <span class="badge badge-warning text-white">{{ $t('reviewing') }}</span>
          </td>
          <td>Junior Highschool | Grade 9</td>
          <td>
            <v-button :native-type="'button'">
              <fa :icon="'eye'" fixed-width />
            </v-button>
            <v-button :native-type="'button'" :type="'danger'">
              <fa :icon="'eye'" fixed-width />
            </v-button>
          </td>
        </tr>
      </tbody>
    </table>
  </card>
</template>

<script>
export default {
  middleware: 'auth',

  metaInfo () {
    return { title: this.$t('home') }
  }
}
</script>
