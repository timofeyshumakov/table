<template>
    <v-app>
      <v-main>
        <v-container>
          <v-row>
            <v-col cols="12">
              <h1 class="text-h4 font-weight-bold mb-6">РАБОЧИЙ СТОЛ СОТРУДНИКА</h1>
            </v-col>
          </v-row>

          <!-- Раздел РАБОЧИЙ СТОЛ ОКК -->
          <v-row>
            <v-col cols="12">
              <h2 class="section-title">РАБОЧИЙ СТОЛ ОКК</h2>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/crm/lead/list/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="primary">mdi-account-group</v-icon>
                  <h3 class="text-h6 mt-2">CRM Лиды</h3>
                  <p class="text-caption mt-2">Управление лидами</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>

          <!-- Раздел Б2С -->
          <v-row>
            <v-col cols="12">
              <h2 class="section-title">Б2С</h2>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/bi/dashboard/detail/153/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="green">mdi-chart-bar</v-icon>
                  <h3 class="text-h6 mt-2">Отчет % качества Б2С</h3>
                  <p class="text-caption mt-2">Анализ качества работы</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/crm/reports/report/view/3207/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="green">mdi-file-chart</v-icon>
                  <h3 class="text-h6 mt-2">Универсальный отчет Б2С</h3>
                  <p class="text-caption mt-2">Комплексная аналитика</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/crm/reports/report/view/3735/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="green">mdi-alert-circle</v-icon>
                  <h3 class="text-h6 mt-2">Отчет "Брошенки"</h3>
                  <p class="text-caption mt-2">Незавершенные сделки</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>

          <!-- Раздел Сервис -->
          <v-row>
            <v-col cols="12">
              <h2 class="section-title">Сервис</h2>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/bi/dashboard/detail/169/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="orange">mdi-chart-pie</v-icon>
                  <h3 class="text-h6 mt-2">Отчет % качества Сервис</h3>
                  <p class="text-caption mt-2">Качество сервисных услуг</p>
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <v-card 
                class="dashboard-card pa-4"
                @click="openLink('https://ortonica.bitrix24.ru/crm/reports/report/view/3295/')"
              >
                <v-card-text class="text-center">
                  <v-icon size="48" color="orange">mdi-file-document</v-icon>
                  <h3 class="text-h6 mt-2">Универсальный отчет Сервис</h3>
                  <p class="text-caption mt-2">Аналитика сервисного отдела</p>
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>

          <!-- Раздел ПРМ -->
          <v-row>
            <v-col cols="12">
              <h2 class="section-title">ПРМ</h2>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <a
                  href="https://ortonica.bitrix24.ru/marketplace/app/363/"
                  target="_blank"
                  class="card-link"
              >
                <v-card class="dashboard-card pa-4">
                  <v-card-text class="text-center">
                    <v-icon size="48" color="purple">mdi-puzzle</v-icon>
                    <h3 class="text-h6 mt-2">ПРМ</h3>
                    <p class="text-caption mt-2">Приложение постановки плана развития менеджеров</p>
                  </v-card-text>
                </v-card>
              </a>
            </v-col>
          </v-row>

          <!-- Раздел База знаний -->
          <v-row>
            <v-col cols="12">
              <h2 class="section-title">База знаний</h2>
            </v-col>
            <v-col cols="12" sm="6" md="4">
              <a
                  href="https://ortonica.bitrix24.ru/knowledge/baza_znaniy_OKK/"
                  target="_blank"
                  class="card-link"
              >
                <v-card class="dashboard-card pa-4">
                  <v-card-text class="text-center">
                    <v-icon size="48" color="teal">mdi-book-open-variant</v-icon>
                    <h3 class="text-h6 mt-2">База знаний</h3>
                    <p class="text-caption mt-2">Корпоративная документация</p>
                  </v-card-text>
                </v-card>
              </a>
            </v-col>
          </v-row>
        </v-container>
      </v-main>
    </v-app>
</template>

<script>
export default {
  methods: {
    openLink(url) {
      window.open(url, '_blank');
    }
  }
}
</script>

<style>
.card-link {
  text-decoration: none;
  display: block;
}

.dashboard-card {
  cursor: pointer;
  transition: transform 0.2s;
  height: 100%;
}

.dashboard-card:hover {
  transform: translateY(-5px);
}

.section-title {
  border-bottom: 2px solid #eee;
  padding-bottom: 8px;
  margin-bottom: 16px;
}

#app .text-caption {
  font-size: 1rem !important;
}
</style>