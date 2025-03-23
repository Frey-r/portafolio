<script setup>
import PortfolioItem from "@/components/PortfolioItem.vue";
import ExperienceItem from "@/components/ExperienceItem.vue";
import ProjectItem from "@/components/ProjectItem.vue";
import TechCard from "@/components/TechCard.vue";
import ProfileIcon from "@/components/icons/IconProfile.vue";
import PortfolioIcon from "@/components/icons/IconPortfolio.vue";
import ExperienceIcon from "@/components/icons/IconExperience.vue";
import PandasIcon from "@/components/icons/IconPandas.vue";
import SQLiteIcon from "@/components/icons/IconSQLite.vue";
import SeleniumIcon from "@/components/icons/IconSelenium.vue";
import FastAPIIcon from "@/components/icons/IconFastAPI.vue";
import GithubIcon from "@/components/icons/IconGithub.vue";
import PoetryIcon from "@/components/icons/IconPoetry.vue";
import PythonIcon from "@/components/icons/IconPython.vue";
</script>

<template>
  <PortfolioItem>
    <template #icon>
      <ProfileIcon />
    </template>
    <template #heading>
      Sobre Mi
    </template>
    <template #content>
      <p>
        <span>Desarrollador desde los 16 años, con casi tres años de experiencia profesional en
Idok, empresa líder en optimización de procesos de gestión de negocios y
tecnologías de identificación digital y firma electrónica para personas, empresas
y organizaciones.</span><span>
Me adapto con facilidad a entornos cambiantes y disfruto del trabajo en equipo,
aunque también tengo la habilidad para desempeñarme de manera autónoma.</span><span>
Soy autodidacta por naturaleza y busco constantemente nutrirme de conocimiento a través de cursos,
lecturas y el intercambio con colegas.
Mi objetivo es enriquecer mi práctica profesional y aportar soluciones de valor en cada proyecto.</span>
      </p>
    </template>
  </PortfolioItem>
  <PortfolioItem>
    <template #icon>
      <ExperienceIcon />
    </template>
    <template #heading>
      Experiencia
    </template>
    <template #content>
      <ExperienceItem :isOpen="true">
        <template #heading>
          <div>Desarrollador Backend</div>
        </template>
        <template #heading-boldest>
          <span>Idok | Abril 2022 – actualidad</span>
        </template>
        <template #exp-content>
          <p>
            Contratado inicialmente como QA, me encargué de crear, documentar y
automatizar pruebas para diversos servicios, empleando Python y Selenium.
Poco después, fui trasladado al equipo de Backend, donde actualmente
desarrollo y mantengo microservicios utilizando Java 8 y Spring Boot. En este rol,
he trabajado en la modificación, adaptación y creación de microservicios de
autenticación y firma digital para clientes de sectores públicos y privados,
incluyendo municipios, bancos y otras organizaciones.
          </p>
        </template>
        <template #items-achievements>
          <li>
            Microservicios: Desarrollé microservicios personalizados para la
autenticación y firma digital, adaptados a las necesidades de cada cliente.
          </li>
          <li>
            Sistema de reportería automatizada: Implementé un sistema de
reportería para el área comercial, desde la arquitectura y base de datos
hasta el despliegue en AWS. Este sistema permite monitorear
transacciones de firma, compra de productos y el uso de servicios de
terceros.
          </li>
          <li>
            Implementación en AWS: Configuré y gestioné la infraestructura en AWS,
asegurando la eficiencia y escalabilidad del servicio de reportería.
Desplegué actualizaciones de servicios de firma alojados en EC2.
          </li>
        </template>
        <template #items-technologies>
          <li>
            <details class="tech-details">
              <summary>
                Java 8:
              </summary>
              <ul>
                <li>
                  Spring Boot (Framework de backend)
                </li>
                <li>
                  Maven (Gestión de dependencias)
                </li>
              </ul>
            </details>
          </li>
          <li>
            <details class="tech-details">
              <summary>
                Python:
              </summary>
              <ul>
                <li>
                  Poetry (Gestión de paquetes)
                </li>
                <li>
                  Selenium (Pruebas automatizadas)
                </li>
                <li>
                  Requests (Pruebas automatizadas)
                </li>
                <li>
                  Pandas (Procesamiento de datos para el área comercial)
                </li>
              </ul>
            </details>
          </li>
          <li>
            <details class="tech-details">
              <summary>
                MySQL:
              </summary>
              <ul>
                <li>
                  Base de datos para reportería y servicios de firma digital.
                </li>
              </ul>
            </details>
          </li>
          <li>
            <details class="tech-details">
              <summary>
                AWS:
              </summary>
              <ul>
                <li>
                  EC2 (Servidores para servicios de firma)
                </li>
                <li>
                  SQS (Sistema de colas para ejecución asincrónica)
                </li>
                <li>
                  RDS (Host de la base de datos para el servicio de reportería)
                </li>
              </ul>
            </details>
          </li>
        </template>
      </ExperienceItem>
    </template>
  </PortfolioItem>
  <PortfolioItem>
    <template #icon>
      <PortfolioIcon />
    </template>
    <template #heading>
      Portafolio
    </template>
    <template #content>
      <ProjectItem>
        <template #heading>
          Scrapper para ofertas de inmuebles:
        </template>
        <template #technology>
          <TechCard>
            <template #icon>
              <PandasIcon />
            </template>
            <template #content>
              Pandas
            </template>
          </TechCard>
          <TechCard>
            <template #icon>
              <SQLiteIcon />
            </template>
            <template #content>
              SQLite
            </template>
          </TechCard>
          <TechCard>
            <template #icon>
              <SeleniumIcon  />
            </template>
            <template #content>
              Selenium
            </template>
          </TechCard>
        </template>
        <template #link>
          <a href="https://github.com/Frey-r/ApartmentRentScraperBot" class="github-link">
            <i>
              <GithubIcon />
            </i>
            <span>Ver en Github</span>
          </a>
        </template>
        <template #description>
          <p>
            Este scraper está diseñado para:
          </p>
          <ul>
            <li>Rastrear propiedades en alquiler dentro de rangos de precios y ubicaciones específicas.</li>
            <li>Almacenar detalles de las propiedades, incluyendo precio, ubicación y disponibilidad.</li>
            <li>Monitorear cambios en los listados a lo largo del tiempo.</li>
            <li>Mantener un historial de los listados de propiedades.</li>
          </ul>
        </template>
      </ProjectItem>
      <ProjectItem>
        <template #heading>
          Bot de Discord para competición de Elo:
        </template>
        <template #technology>
          <TechCard>
            <template #icon>
              <PoetryIcon />
            </template>
            <template #content>
              Poetry
            </template>
          </TechCard>
          <TechCard>
            <template #icon>
              <PythonIcon />
            </template>
            <template #content>
              Python
            </template>
          </TechCard>
          <TechCard>
            <template #icon>
              <SQLiteIcon />
            </template>
            <template #content>
              SQLite
            </template>
          </TechCard>
          <TechCard>
            <template #icon>
              <FastAPIIcon />
            </template>
            <template #content>
              FastAPI
            </template>
          </TechCard>
        </template>
        <template #link>
          <a href="https://github.com/Frey-r/EloRace" class="github-link">
            <i>
              <GithubIcon />
            </i>
            <span>Ver en Github</span>
          </a>
        </template>
        <template #description>
          <p>
            Este bot está diseñado para:
          </p>
          <ul>
            <li>Conectarse a la API de Riot Games para obtener información de los jugadores.</li>
            <li>Crear carreras de Elo, a modo de competencia para los jugadores.</li>
            <li>Monitorear cambios en los jugadores a lo largo del tiempo.</li>
          </ul>
        </template>
      </ProjectItem>
    </template>
  </PortfolioItem>
</template>

<style scoped>
  p{
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
  }
  .github-link{
    display: flex;
    gap: 0.6rem;
    align-items: center;
    & i{
      height: 1.5rem;
      width: 1.5rem;
      display: flex;
      place-items: center;
      place-content: center;
      background-color: var(--vt-c-white);
      border-radius: 8px;
    }
  }
</style>