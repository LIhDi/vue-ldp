<template>
  <div>
    <a href="https://api.whatsapp.com/send/?phone=5521966591786&text&type=phone_number&app_absent=0">
      <q-icon class="fixed-bottom-right z-top q-pa-md" size="4em" name="img:whatsapp-56x56.webp" /></a>
    <div v-if="$q.screen.lt.md">
      <a href="https://pay.kiwify.com.br/Gqu1EqM"><q-img rel="preload" src="img/640x360.webp"/></a>
    </div>
    <div v-if="$q.screen.md">
      <a href="https://pay.kiwify.com.br/Gqu1EqM"><q-img rel="preload" src="img/1024x576.webp"/></a>
    </div>
      <div v-if="$q.screen.lg">
        <a href="https://pay.kiwify.com.br/Gqu1EqM"><q-img rel="preload" src="img/1600x900.webp"/></a>
    </div>
    <div v-if="($q.screen.xl || $q.screen.gt.xl)">
      <a href="https://pay.kiwify.com.br/Gqu1EqM"><q-img rel="preload" src="img/1920x1080.webp"/></a>
    </div>
    <div class="row q-px-xl q-pb-xl justify-around bg-grey-8 q-gutter-y-xl">
      <div class="col-12 q-pa-md text-center">
        <div class="text-h4 q-mt-md text-weight-bolder">Como funciona o nosso desafio 30 dias de emagrecimento</div>
        <div class="text-subtitle1 text-weight-medium q-mt-md">
        Todo o conteúdo foi cuidadosamente elaborado por profissionais da aréa da saúde, para que você consiga transformar seu corpo, respeitando seus limites, idade e estilo de vida.
      </div>
      </div>
      <div id="borda-circular" class="col-lg-4 col-md-6 col-sm-6 col-xs-12" v-for="i in beneficiosCards" :key="i.id">
        <div class="row">
          <div class="col-md-5 col-sm-12 col-xs-12 text-center q-pb-md">
            <div>
              <q-icon color="warning" size="6.4em" :name="i.imagem" />
              <q-btn
                fab
                color="info"
                size="15px"
                class="relative"
                style="top: 0; right: 0px; transform: translateY(-50%);">
                <div style="fontSize: 30px;" class="text-white text-weight-bolder">{{i.id}}</div>
              </q-btn>
            </div>
          </div>
          <div class="col-md-7 col-sm-12 col-xs-12">
            <div class="text-h5 text-weight-bold q-pl-md">{{i.titulo}}</div>
            <div class="text-subtitle2 q-pl-md">{{i.subtitulo}}</div>
          </div>
        </div>
      </div>
    </div>
    <div class="row justify-around q-py-xl q-gutter-y-lg">
      <div class="col-12 text-h4 text-weight-bolder text-center">
        Melhor método de perda de peso do Brasil
      </div>
      <div class="col-12 text-subtitle2 text-weight-medium text-center">
        Curso atualizado com foco no emagrecimento com saúde
      </div>
      <div class="col-md-12 col-sm-12 col-xs-12 q-px-xl text-center">
        <q-card flat bordered>
          <q-card-section class="bg-warning">
            <div class="text-h6 q-mb-xs text-weight-bolder">Curso Completo - 2023</div>
            <div class="text-caption text-grey text-weight-medium q-ml-sm">Cardápio montado por especialistas + Flexível + Fácil de fazer + Perda de peso garantida</div>
            <q-chip square size="lg" class="absolute text-white text-weight-bolder" color="red" style="top: 0; right: 12px; transform: translateY(-50%);">
                50% DE DESCONTO
            </q-chip>
          </q-card-section>
          <q-card-section>
            <div class="row">
              <div class="col-md-5 col-sm-5 col-xs-12 text-center">
                <q-card-section>
                  <div>
                    <q-chip size="35px" square>
                      <q-avatar q-avatar icon="bookmark" color="red" text-color="white" />
                      50% OFF
                    </q-chip>
                  </div>
                  <div class="text-subtitle1 text-grey q-pa-sm">
                    <span class="text-grey-4" style="text-decoration: line-through;">De: R$ 179,90</span>
                    <span class="q-ml-sm">Por: R$ 89,90</span>
                  </div>
                  <div class="text-subtitle2 text-weight-medium q-pa-sm">Ou em apenas 12x</div>
                  <div class="text-h2 text-weight-bolder q-pb-lg">R$ 9,03</div>
                  <q-btn
                  @click="comprarCurso()"
                    color="positive"
                    label="COMPRE AGORA"
                    size="30px"
                  />
                </q-card-section>
              </div>
              <div class="col-md-6 col-sm-6 col-xs-12">
                <q-card-section class="col-md-6 col-sm-6 col-xs-12 flex flex-center">
                  <q-img
                    class="rounded-borders"
                    src="./../assets/images/dieta-ou-exercicio-qual-emagrece-mais.jpg"
                  />
                </q-card-section>
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>
    </div>

    <div class="row justify-around q-pa-xl q-gutter-y-lg bg-grey-8">
      <div class="col-12 text-h4 text-weight-bolder text-center">
        Avaliações de quem já aceitou o desafio
      </div>
      <div class="col-12 text-subtitle2 text-weight-medium text-center">
        Confira o que os clientes que já compraram versões anteriores disseram sobre o desafio.
      </div>
      <div class="col-md-6 col-sm-5 col-xs-12">
          <q-img fit="fill" src="./../assets/images/dieta-e-academia.jpg"/>
          <div class="row q-pa-md q-gutter-y-md">
            <div class="col-6">
              <q-btn outline round size="lg" color="secondary" icon="credit_score" />
              <span class="text-caption text-left text-weight-bold q-ml-sm">PAGUE EM ATÉ 12X</span>
            </div>
            <div class="col-6">
              <q-btn outline round size="lg" color="secondary" icon="tips_and_updates" />
              <span class="text-caption text-left text-weight-bold q-ml-sm">CURSO ATUALIZADO</span>
            </div>
            <div class="col-6">
              <q-btn outline round size="lg" color="secondary" icon="lock_person" />
              <span class="text-caption text-left text-weight-bold q-ml-sm">SITE 100% SEGURO</span>
            </div>
            <div class="col-6">
              <q-btn outline round size="lg" color="secondary" icon="check" />
              <span class="text-caption text-left text-weight-bold q-ml-sm">PERDA DE PESO COM SAÚDE</span>
            </div>
          </div>
        </div>
      <div class="col-md-5 col-sm-5 col-xs-12 q-ml-md">
        <div class="row items-center">
          <span class="text-h5 text-weight-bold">4.6</span>&nbsp;&nbsp;&nbsp;
          <q-rating
            v-model="ratingModel"
            icon="star"
            size="2em"
            color="warning"
            icon-half="star_half"
            readonly
          />
          <div class="text-caption">4.6 de 5 estrelas de acordo com as avaliações dos nossos clientes &nbsp;&nbsp;&nbsp;</div>
        </div>
        <div class="row q-mt-sm" v-for="star in starBars" :key="star.id">
          <div class="col-md-3 col-sm-4 col-xs-4 text">{{star.descricao}}</div>
          <div class="col-md-9 col-sm-8 col-xs-8"><q-linear-progress :aria-label="star.id" rounded size="20px" :value="star.valor" color="warning"/></div>
        </div>
        <q-scroll-area
          class="q-mt-lg"
          visible
          style="height: 300px">
          <div v-for="user in usersFeedbacks" :key="user.id">
            <q-item clickable v-ripple>
              <q-item-section side>
                <q-avatar style="margin-left: -12px" size="48px" color="white" icon="person">
                  <q-badge floating rounded color="green">
                  <q-icon style="font-size: 1rem;" color="warnig" name="verified_user"/>
                </q-badge>
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <div class="row no-wrap items-center">
                  <div class="col text-subtitle1 ellipsis">
                    {{user.nome}}
                    <span class="text-caption">{{` - ${user.data}`}}</span>
                  </div>
                </div>
                <q-item-label><q-rating v-model="user.estrelas" readonly size="16px" /></q-item-label>
                <q-item-label>{{user.mensagem}}</q-item-label>
              </q-item-section>
            </q-item>
          </div>
        </q-scroll-area>
      </div>
    </div>

    <div class="row justify-around q-pa-xl q-gutter-y-lg">
      <div class="col-12 text-h4 text-weight-bolder text-center">
        O que você precisa saber
      </div>
      <div class="col-12 text-subtitle2 text-weight-medium text-center">
        Aqui você encontra as principais dúvidas sobre o Desafio 30 dias
      </div>
      <div class="col-md-12 col-sm-12 col-xs-12 q-pa-md bg-white">
        <q-list bordered class="rounded-borders">
          <q-expansion-item default-opened expand-separator label="Tenho que pagar todos os meses para continuar recebendo o curso atualizado?" caption="Pagamento único">
            <q-card>
              <q-card-section class="text-red">
                Não, o pagamento é efetuado apenas uma vez.
              </q-card-section>
            </q-card>
          </q-expansion-item>
          <q-separator />
      <q-expansion-item expand-separator label="Como continuo recebendo as atualizações do desafio?" caption="Será enviado um coupom para a próxima atualização">
        <q-card>
          <q-card-section>
            Após o pagamento você terá acesso ao desafio completo. Você também terá acesso ao coupom que deverá ser utilizado quando sair a próxima atualização, tornando o curso gratuito.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="E caso eu não goste do curso?" caption="Poderá pedir reembolso">
        <q-card>
          <q-card-section>
            Você terá 7 dias para pedir o reembolso do valor total em caso de insatisfação.          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="Tenho muita dificuldade para emagrecer, porque com esse curso vou conseguir?" caption="A perda de peso é garantida">
        <q-card>
          <q-card-section>
            A perda de peso ao contrário do que dizem não possui nenhum segredo, seguindo os protocolos do curso a perda de peso é garantida.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="Qual a diiferença deste curso para outros?" caption="O nosso curso é o mais utilizado do Brasil">
        <q-card>
          <q-card-section>
            A partir do momento da compra você pode começar imediatamente a seguir o protocolo, como se fosse em uma consulta presencial no nutricinista, não há aulas nem vídeos apenas um protocolo a seguir.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="Nunca fiz nenhuma dieta restritiva ou exercícios, será que eu consigo?" caption="Você será o maior beneficiado com esse curso">
        <q-card>
          <q-card-section>
            Sim, o que entregamos aqui não é uma dieta restritiva mas sim uma reeducação alimentar utilizando alimentos saudavéis e que cabem no bolso. Assim como os exercícios também contêm uma variedade muito grande.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="Não consegui comprar na pré-venda como faço para obter o desconto?" caption="Apenas damos descontos na pré-venda">
        <q-card>
          <q-card-section>
            Apenas damos descontos para clientes que compram na pré-venda e mesmo assim não sabemos se na proxima vamos conseguir manter as mesmas condições de valor e pagamento.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
      <q-expansion-item expand-separator label="De quanto em quanto tempo é realizado o sorteio de R$ 250,00? E como participo?" caption="Ao comprar o curso você já passa a concorrer">
        <q-card>
          <q-card-section>
            Todas as pessoas que comprarem o curso concorrem ao prêmio, o sorteio irá ocorrer sempre um dia após a atualiização do nosso curso, ou seja de 3 em 3 meses.
          </q-card-section>
        </q-card>
      </q-expansion-item>
      <q-separator />
        </q-list>
      </div>
      <q-btn
        @click="comprarCurso()"
        color="positive"
        label="COMPRE AGORA"
        size="lg"
        class="full-width"
      />
    </div>

    <div class="row bg-grey-8 q-pa-xl text-center">
      <div class="col-md-3 col-sm-3 col-xs-12"></div>
      <div class="col-md-4 col-sm-4 col-xs-12">
        <div class="text-h4 text-weight-bolder q-pa-md">
          GARANTIA DE 7 DIAS
        </div>
        <div class="text-subtitle2">
          Está em dúvida se realmente vai funcionar, experimente nossas receitas e planos alimentares por 7 dias.
        </div>
        <div class="text-subtitle1 q-py-lg text-weight-bolder">
          VOCÊ TEM 7 DIAS DE GARANTIA INCONDICIONAL
        </div>
        <div class="text-subtitle2 q-pb-md">
          Se por algum motivo você achar que o desafio não é pra você, é só entrar em contato por um dos nossos canais de comunicação que devolvemos todo o seu dinheiro.
        </div>
      </div>
        <div class="col-md-4 col-sm-4 col-xs-12">
            <q-img
            style="max-width: 320px"
            contain
              src="./../assets/images/garantia.webp"/>
          </div>
    </div>

    <div class="q-py-xl q-px-sm bg-black">
      <div class="row">
        <div class="col-md-4 col-sm-4 col-xs-12">
          <div class="row justify-around">
            <div class="col-md-6 col-sm-6 text-center col-xs-6">
              <q-img style="max-width: 100px" src="./../assets/images/message.png"/>
            </div>
            <div class="col-md-6 col-sm-12 col-xs-12 text-center text-white">
              <div class="text-subtitle2 text-weight-bolder">
                NÓS ENVIAMOS CONTEÚDOS
              </div>
              <div class="text-subtitle2 text-weight-bolder">
                E OFERTAS INCRÍVEIS!
              </div>
              <div class="text-caption">
                Receba em primeira mão dicas, cupons, lançamentos e promoções exclusivas!
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-8 col-sm-8 col-xs-12 q-px-md q-pt-md">
          <div class="row q-gutter-y-sm q-gutter-x-sm">
            <div class="col-md-3 col-sm-12 col-xs-12">
              <div id="borda-circular" class="col-3 bg-white">
                <q-input dark standout stack-label label-color="grey-2" label="Nome" v-model="cliente.nome" />
              </div>
            </div>
            <div class="col-md-6 col-sm-12 col-xs-12">
              <div id="borda-circular" class="col-3 bg-white">
                <q-input dark standout stack-label label-color="grey-2" label="E-mail" v-model="cliente.email" />
              </div>
            </div>
            <div class="col-md-2 col-sm-12 col-xs-12">
              <q-btn
              unelevated
                id="borda-circular"
                @click="cadastrarCliente()"
                color="info"
                label="CADASTRAR"
                class="full-width"
                size="18px"
              />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="row justify-around q-pa-xl q-gutter-y-lg">
      <div class="col-12 text-h4 text-weight-bolder text-center">
        Processo de compra 100% seguro
      </div>
      <div class="col-12 text-subtitle2 text-weight-medium text-center">
        Durante todo o processo seus dados e sua compra estarão seguros
      </div>
      <div id="div-1" class="col-md-5 col-sm-5 col-xs-12 q-pa-md" v-for="item in securityCards" :key="item.id">
        <div class="row">
          <div class="col-6 col-xs-4 text-center">
            <q-icon style="font-size: 6rem;" color="positive" :name="item.icone"/>
          </div>
          <div class="col-6 col-xs-6">
            <div class="text-h5 text-weight-bold text-positive">{{item.titulo}}</div>
            <div class="text-body2">{{item.descricao}}</div>
          </div>
          </div>
      </div>
    </div>
    <div class="row justify-around q-pa-lg q-gutter-y-lg bg-grey-8">
      <div class="col-md-8 col-sm-12 col-xs-12 q-pa-md">
          <div class="text-left text-weight-bold">
            Copyright © DESAFIO30DIAS. Todos os direitos reservados.
          </div>
          <div class="text-caption text-grey-2 q-mt-md">
            Todo o conteúdo da página incluindo fotos, imagens, logotipos e layout aqui veículados são de propriedade exclusiva da DESAFIO30DIAS. É vedada qualquer reprodução, total ou parcial, de qualquer elemento da página sem a autorização. A violação de qualquer direito mencionado implicará na responsabilização cível e criminal nos termos da Lei.
          </div>
          <div class="text-caption text-grey-2 q-mt-md">
            Preços e condições de pagamento exclusivos para compras via internet. Vendas sujeitas à análise e confirmação de dados. Os valores dos produtos podem ser alterados a qualquer momento, sem aviso prévio.
          </div>
      </div>
      <div class="col-md-4 col-sm-12 col-xs-12 q-pa-md">
        <div class="text-left text-weight-bold">
          Certificados de Segurança da Página
        </div>
        <div>
          <q-img style="max-width: 150px" src="./../assets/images/certificado.png"/>
          <q-img class="q-ml-sm" style="max-width: 90px" src="./../assets/images/compra-segura.png"/>
          <q-img class="q-ml-sm" style="max-width: 100px" src="./../assets/images/reclame-aqui.png"/>
        </div>
        <div>
          <q-img style="max-width: 120px" src="./../assets/images/google-site-seguro.png"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { useQuasar } from 'quasar'
import { openURL } from 'quasar'
import { defineComponent } from 'vue'
  export default defineComponent({
    name: 'DefaultPage',
    setup () {
      const $q = useQuasar()

      return {
      showNotif () {
        $q.notify({
          message: 'Cadastro realizado com sucesso.',
          color: 'positive'
        })
      }
    }
  },
    data () {
    return {
      cliente: {nome: '', email: ''},
      ratingModel: 4.6,
      beneficiosCards: [
        { id: '1', imagem: 'img:goal-90x90.webp', titulo: 'O Desafio', subtitulo: 'O nosso Desafio 30 dias contém várias indicações de cardápio, mas também um passo a passo detalhado de como montar o seu personalizado com diversas receitas.' },
        { id: '2', imagem: 'img:clipboard-90x90.webp', titulo: 'Siga o protocolo', subtitulo: 'Com uma variedade de alimentos e receitas, todo o cardápio pode ser totalmente adaptado conforme a sua necessidade, não há que sentir peso na consciência o desafio é simples é eficaz.' },
        { id: '3', imagem: 'img:calendar10-90x90.webp', titulo: '10 dias', subtitulo: 'Na fase inicial o seu corpo irá perceber a mudança de hábitos e você pode perder até 7 kg só nesta primeira fase.' },
        { id: '4', imagem: 'img:calendar20-90x90.webp', titulo: '20 dias', subtitulo: 'A perda de peso se intensifica devido aos novos hábitos, o corpo já não armazena gordura e começa a transforma-la em energia e consequentemente você percebe a perda de medidas, aumento de energia e disposição no seu dia a dia.' },
        { id: '5', imagem: 'img:calendar30-90x90.webp', titulo: '30 dias', subtitulo: 'Você chegou na fase final, se chegou até aqui você verá que o desafio realmente mudou a sua vida, com a perda de peso e aumento da autoestima você se sente pronta para novos desafios.' },
        { id: '6', imagem: 'img:slim-90x90.webp', titulo: 'Atualização', subtitulo: 'Apenas nos 30 dias de desafio você já vai obter uma grande perda de peso pondendo ser superior a 15kg. Mas caso ainda precise perder mais peso, nós garantimos a atualização constante do desafio acelerando ainda mais o processo de emagrecimento pois o corpo receberá novos estimulos mensalmente e consequentemente atingindo o seu objetivo. ' }
      ],
      starBars: [
        { id: '1', descricao: 'Excelente', valor: 0.8 },
        { id: '2', descricao: 'Muito Bom', valor: 0.15 },
        { id: '3', descricao: 'Bom', valor: 0.18 },
        { id: '4', descricao: 'Ruim', valor: 0 },
        { id: '5', descricao: 'Muito Ruim', valor: 0 }
      ],
      securityCards: [
        { id: '1', icone: 'lock_person', titulo: 'Dados Pessoais', descricao: 'Dados totalmente sigilosos e não compartilhados.'},
        { id: '2', icone: 'verified_user', titulo: 'Site Confiável', descricao: 'Site monitorado por empresas de segurança digital.'},
        { id: '3', icone: 'lock', titulo: 'Dados Financeiros', descricao: 'Apenas para uso no momento do pagamento.'},
        { id: '4', icone: 'check_box', titulo: 'Entrega Garantida', descricao: 'Produto entregue logo após a confirmação do pagamento.'}
      ],
      usersFeedbacks: [
        { id: '1', estrelas: 5, nome: 'larialbino', mensagem: 'Já tinha comprado a primeira versão lá em 2019, no total foram 15 kg !!! esse treino está demais parabéns!', data: '05/07/2022' },
        { id: '2', estrelas: 4, nome: 'nathfranca', mensagem: 'Achei que não ia conseguir e agora estou fazendo todos os dias e a dieta está maravilhosa!!', data: '06/07/2022' },
        { id: '3', estrelas: 5, nome: 'andre22', mensagem: 'Dei o curso para a minha esposa e me surpreendi, acabou que eu e ela aceitamos o desafio, sensacional o material!', data: '23/08/2022' },
        { id: '4', estrelas: 4, nome: 'amandaspgomes', mensagem: 'Comprei a versão 2022 e já quero fazer tudo, super animada vcs são d+++', data: '24/11/2022' },
        { id: '5', estrelas: 5, nome: 'diogomene06', mensagem: 'Recebi o material tem quase um mês, esperei para realmente vir dar a minha opnião, muito obrigada por criarem esse conteúdo.', data: '28/11/2022' },
        { id: '6', estrelas: 5, nome: 'maria15pereira', mensagem: '😍😍😍😍😍😍', data: '06/11/2022' },
        { id: '7', estrelas: 5, nome: 'nandasilva64', mensagem: 'Só quero agradecer de coração mesmo, graças ao curso consegui melhorar a quallidade de vida, obrigada.', data: '23/11/2022' },
        { id: '8', estrelas: 5, nome: 'vania63silva', mensagem: 'Top👏😍', data: '29/11/2022' }
      ]
    }
  },
  methods: {
    comprarCurso () {
      openURL("https://pay.kiwify.com.br/Gqu1EqM")
    },
    cadastrarCliente () {
      this.showNotif()
      this.cliente = {}
    }
  }
})
</script>

<style lang="scss">
#div-1{
  background: #eff6e9;
  border-radius: 10px;
  border: 1px solid #afd493
}
#borda-circular{
  border-radius: 5px;
}
.q-field--standout .q-field__control{
  height: 46px;
}
.q-field--dark .q-field__native{
  color: black
}
</style>
