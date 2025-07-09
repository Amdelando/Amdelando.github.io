npx create-next-app nexusbm --typescript
cd nexusbm
npm install tailwindcss framer-motion react-icons @types/node --save
├── components/
│   ├── Header.tsx
│   ├── Footer.tsx
│   ├── ServiceCard.tsx
│   ├── Testimonial.tsx
│   └── WhatsAppButton.tsx
├── pages/
│   ├── index.tsx (Home)
│   ├── sobre.tsx
│   ├── servicos.tsx
│   ├── portfolio.tsx
│   └── contato.tsx
├── public/
│   ├── images/
│   └── favicon.ico
├── styles/
│   └── globals.css
└── tsconfig.json
import type { AppProps } from 'next/app'
import { ThemeProvider } from 'next-themes'
import '../styles/globals.css'
import Head from 'next/head'

function MyApp({ Component, pageProps }: AppProps) {
  return (
    <ThemeProvider attribute="class">
      <Head>
        <title>NexusBM - Marketing Digital e Tecnologia</title>
        <meta name="description" content="Soluções em gestão de tráfego pago, criação de sites e marketing digital" />
        <link rel="icon" href="/favicon.ico" />
      </Head>
      <Component {...pageProps} />
    </ThemeProvider>
  )
}

export default MyApp
import { motion } from 'framer-motion'
import Head from 'next/head'
import Header from '../components/Header'
import ServiceCard from '../components/ServiceCard'
import Testimonial from '../components/Testimonial'
import WhatsAppButton from '../components/WhatsAppButton'

const Home = () => {
  const services = [
    {
      title: 'Gestão de Tráfego Pago',
      description: 'Campanhas otimizadas no Facebook Ads e Google Ads para trazer clientes qualificados.',
      icon: '📈'
    },
    {
      title: 'Criação de Sites',
      description: 'Sites modernos, rápidos e otimizados para conversão.',
      icon: '💻'
    },
    {
      title: 'Copywriting',
      description: 'Textos persuasivos que vendem seu produto ou serviço.',
      icon: '✍️'
    }
  ]

  const testimonials = [
    {
      name: 'Carlos Silva',
      company: 'Empresa XYZ',
      text: 'A NexusBM transformou nosso negócio com campanhas de tráfego que realmente convertem.',
      rating: 5
    }
  ]

  return (
    <div className="min-h-screen bg-gray-50">
      <Head>
        <title>NexusBM - Marketing Digital de Resultados</title>
      </Head>

      <Header />
      <WhatsAppButton />

      {/* Hero Section */}
      <section className="pt-32 pb-20 px-4 bg-gradient-to-r from-blue-900 to-blue-700 text-white">
        <div className="container mx-auto text-center">
          <motion.h1 
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8 }}
            className="text-4xl md:text-6xl font-bold mb-6"
          >
            Transforme seu negócio com <span className="text-blue-300">marketing digital</span>
          </motion.h1>
          
          <motion.p 
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8, delay: 0.2 }}
            className="text-xl md:text-2xl mb-8 max-w-3xl mx-auto"
          >
            Soluções completas em gestão de tráfego, criação de sites e copywriting para alavancar suas vendas.
          </motion.p>
          
          <motion.div
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8, delay: 0.4 }}
          >
            <a 
              href="#contato" 
              className="bg-blue-400 hover:bg-blue-300 text-blue-900 font-bold py-3 px-8 rounded-full text-lg transition inline-block"
            >
              Fale conosco
            </a>
          </motion.div>
        </div>
      </section>

      {/* Services Section */}
      <section className="py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-blue-900">
            Nossos <span className="text-blue-600">Serviços</span>
          </h2>
          
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            {services.map((service, index) => (
              <ServiceCard 
                key={index}
                title={service.title}
                description={service.description}
                icon={service.icon}
                delay={index * 0.1}
              />
            ))}
          </div>
        </div>
      </section>

      {/* Testimonials Section */}
      <section className="py-20 px-4 bg-gray-100">
        <div className="container mx-auto">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-blue-900">
            O que nossos <span className="text-blue-600">clientes</span> dizem
          </h2>
          
          <div className="max-w-4xl mx-auto">
            {testimonials.map((testimonial, index) => (
              <Testimonial 
                key={index}
                name={testimonial.name}
                company={testimonial.company}
                text={testimonial.text}
                rating={testimonial.rating}
              />
            ))}
          </div>
        </div>
      </section>

      {/* CTA Section */}
      <section id="contato" className="py-20 px-4 bg-blue-900 text-white">
        <div className="container mx-auto text-center">
          <h2 className="text-3xl md:text-4xl font-bold mb-6">
            Pronto para transformar seu negócio?
          </h2>
          <p className="text-xl mb-8 max-w-2xl mx-auto">
            Entre em contato agora mesmo e vamos conversar sobre como podemos ajudar você.
          </p>
          <a 
            href="https://wa.me/5511999999999?text=Olá%20NexusBM,%20gostaria%20de%20saber%20mais%20sobre%20seus%20serviços"
            target="_blank"
            rel="noopener noreferrer"
            className="bg-white hover:bg-gray-100 text-blue-900 font-bold py-3 px-8 rounded-full text-lg transition inline-block"
          >
            Falar no WhatsApp
          </a>
        </div>
      </section>

      <Footer />
    </div>
  )
}

export default Home
import { motion } from 'framer-motion'
import Head from 'next/head'
import Header from '../components/Header'
import ServiceCard from '../components/ServiceCard'
import Testimonial from '../components/Testimonial'
import WhatsAppButton from '../components/WhatsAppButton'

const Home = () => {
  const services = [
    {
      title: 'Gestão de Tráfego Pago',
      description: 'Campanhas otimizadas no Facebook Ads e Google Ads para trazer clientes qualificados.',
      icon: '📈'
    },
    {
      title: 'Criação de Sites',
      description: 'Sites modernos, rápidos e otimizados para conversão.',
      icon: '💻'
    },
    {
      title: 'Copywriting',
      description: 'Textos persuasivos que vendem seu produto ou serviço.',
      icon: '✍️'
    }
  ]

  const testimonials = [
    {
      name: 'Carlos Silva',
      company: 'Empresa XYZ',
      text: 'A NexusBM transformou nosso negócio com campanhas de tráfego que realmente convertem.',
      rating: 5
    }
  ]

  return (
    <div className="min-h-screen bg-gray-50">
      <Head>
        <title>NexusBM - Marketing Digital de Resultados</title>
      </Head>

      <Header />
      <WhatsAppButton />

      {/* Hero Section */}
      <section className="pt-32 pb-20 px-4 bg-gradient-to-r from-blue-900 to-blue-700 text-white">
        <div className="container mx-auto text-center">
          <motion.h1 
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8 }}
            className="text-4xl md:text-6xl font-bold mb-6"
          >
            Transforme seu negócio com <span className="text-blue-300">marketing digital</span>
          </motion.h1>
          
          <motion.p 
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8, delay: 0.2 }}
            className="text-xl md:text-2xl mb-8 max-w-3xl mx-auto"
          >
            Soluções completas em gestão de tráfego, criação de sites e copywriting para alavancar suas vendas.
          </motion.p>
          
          <motion.div
            initial={{ opacity: 0, y: 20 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ duration: 0.8, delay: 0.4 }}
          >
            <a 
              href="#contato" 
              className="bg-blue-400 hover:bg-blue-300 text-blue-900 font-bold py-3 px-8 rounded-full text-lg transition inline-block"
            >
              Fale conosco
            </a>
          </motion.div>
        </div>
      </section>

      {/* Services Section */}
      <section className="py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-blue-900">
            Nossos <span className="text-blue-600">Serviços</span>
          </h2>
          
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            {services.map((service, index) => (
              <ServiceCard 
                key={index}
                title={service.title}
                description={service.description}
                icon={service.icon}
                delay={index * 0.1}
              />
            ))}
          </div>
        </div>
      </section>

      {/* Testimonials Section */}
      <section className="py-20 px-4 bg-gray-100">
        <div className="container mx-auto">
          <h2 className="text-3xl md:text-4xl font-bold text-center mb-16 text-blue-900">
            O que nossos <span className="text-blue-600">clientes</span> dizem
          </h2>
          
          <div className="max-w-4xl mx-auto">
            {testimonials.map((testimonial, index) => (
              <Testimonial 
                key={index}
                name={testimonial.name}
                company={testimonial.company}
                text={testimonial.text}
                rating={testimonial.rating}
              />
            ))}
          </div>
        </div>
      </section>

      {/* CTA Section */}
      <section id="contato" className="py-20 px-4 bg-blue-900 text-white">
        <div className="container mx-auto text-center">
          <h2 className="text-3xl md:text-4xl font-bold mb-6">
            Pronto para transformar seu negócio?
          </h2>
          <p className="text-xl mb-8 max-w-2xl mx-auto">
            Entre em contato agora mesmo e vamos conversar sobre como podemos ajudar você.
          </p>
          <a 
            href="https://wa.me/5511999999999?text=Olá%20NexusBM,%20gostaria%20de%20saber%20mais%20sobre%20seus%20serviços"
            target="_blank"
            rel="noopener noreferrer"
            className="bg-white hover:bg-gray-100 text-blue-900 font-bold py-3 px-8 rounded-full text-lg transition inline-block"
          >
            Falar no WhatsApp
          </a>
        </div>
      </section>

      <Footer />
    </div>
  )
}

export default Home
import { motion } from 'framer-motion'
import { FaWhatsapp } from 'react-icons/fa'

const WhatsAppButton = () => {
  return (
    <motion.a
      href="https://wa.me/5511999999999?text=Olá%20NexusBM,%20gostaria%20de%20saber%20mais%20sobre%20seus%20serviços"
      target="_blank"
      rel="noopener noreferrer"
      className="fixed bottom-6 right-6 bg-green-500 text-white p-4 rounded-full shadow-lg z-50"
      whileHover={{ scale: 1.1 }}
      whileTap={{ scale: 0.9 }}
      initial={{ opacity: 0, y: 20 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ delay: 1 }}
    >
      <FaWhatsapp size={28} />
    </motion.a>
  )
}

export default WhatsAppButton
npm run dev