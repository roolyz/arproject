import React, { useState, useEffect } from 'react';
import { 
  Key, 
  Clock, 
  Star, 
  MapPin, 
  Phone,
  Shield,
  Truck,
  MessageCircle,
  ChevronDown,
  Sparkles,
  Zap,
  Lock,
  MapIcon as WhatsappIcon
} from 'lucide-react';

const slides = [
  {
    url: "https://i.ibb.co.com/Cpqr65cB/gambar1.jpg",
    title: "Kunci hIlang? No Worries!",
    subtitle: "Duplikat kunci instan, ga pake lama 🔑✨"
  },
  {
    url: "https://i.ibb.co.com/Q3kn0WLQ/gambar2.jpg",
    title: "Mobile Service 24/7",
    subtitle: "Kapanpun dimanapun, kita siap gas! 🏃‍♂️💨"
  },
  {
    url: "https://i.ibb.co.com/8LgB2YXR/gambar3.jpg",
    title: "Trusted & Reliable",
    subtitle: "Udah ratusan customer happy with our service! 💯"
  }
];

const testimonials = [
  {
    name: "Helni Anggraeni",
    text: "Gila sih ini, murce garcep, hasilnya juga gak kaleng kaleng rekomended bgt pokoknya Thanks bang bantuannya 🙌",
    rating: 5,
    tag: "Verified Customer ✓"
  },
  {
    name: "Abdu Rahman",
    text: "kunci hilang malem malem abis lebaran bisa dipanggil ke rumah untungnya. abis lebaran segala ilang, untung bisa dikerjakan satset🙏😁",
    rating: 5,
    tag: "Verified Customer ✓"
  },
  {
    name: "Firsky Ogest",
    text: "Pengerjaan cepat dan rapih... dan juga bisa datang ke tempat lokasi, fast respon... pokoknya bagus banget deh 💯",
    rating: 5,
    tag: "Verified Customer ✓"
  }
];

const faqs = [
  {
    question: "Berapa lama sih prosesnya?",
    answer: "Santuy, proses duplikasi kunci cepet kok. Secepat bikin Indomie! 🍜"
  },
  {
    question: "Bisa panggil malem-malem ga?",
    answer: "Bisa banget! Kita available 24/7. Malem-malem tetep gas! 🌙"
  },
  {
    question: "Kunci apa aja yang bisa diduplikat?",
    answer: "Literally everything! Kunci rumah, mobil, motor, brankas, dll. You name it, we duplicate it! 🔐"
  },
  {
    question: "Ada garansi ga sih?",
    answer: "Tentu dong! Kita kasih garansi kalo ada masalah dengan hasil duplikat. Langsung chat aja kalo ada apa-apa! 💪"
  }
];

const benefits = [
  {
    icon: Zap,
    title: "Fast Response",
    desc: "Chat atau telpon aja! ⚡️"
  },
  {
    icon: Shield,
    title: "Pro Banget",
    desc: "Hasil premium 💪"
  },
  {
    icon: Sparkles,
    title: "Premium Quality",
    desc: "Full garansi ✨"
  },
  {
    icon: Truck,
    title: "Mobile Service",
    desc: "Dateng ke lokasi 🚗"
  }
];

function App() {
  const [currentSlide, setCurrentSlide] = useState(0);
  const [currentTestimonial, setCurrentTestimonial] = useState(0);
  const [openFaq, setOpenFaq] = useState<number | null>(null);

  useEffect(() => {
    const timer = setInterval(() => {
      setCurrentSlide((prev) => (prev + 1) % slides.length);
    }, 5000);
    return () => clearInterval(timer);
  }, []);

  useEffect(() => {
    const timer = setInterval(() => {
      setCurrentTestimonial((prev) => (prev + 1) % testimonials.length);
    }, 4000);
    return () => clearInterval(timer);
  }, []);

  return (
  <div className="w-full overflow-x-hidden">
    <div className="min-h-screen bg-black text-white">
      {/* Hero Section */}
      <div className="relative h-screen">
        {slides.map((slide, index) => (
          <div
            key={index}
            className={`absolute inset-0 transition-all duration-1000 ${
              index === currentSlide ? 'opacity-100 scale-100' : 'opacity-0 scale-105'
            }`}
          >
            <div className="absolute inset-0 bg-gradient-to-b from-black/30 via-black/50 to-black" />
            <img
              src={slide.url}
              alt={slide.title}
              className="w-full h-full object-cover"
            />
            <div className="absolute inset-0 flex flex-col items-center justify-center text-center p-4">
              <h1 className="text-5xl md:text-7xl font-bold mb-4 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
                {slide.title}
              </h1>
              <p className="text-xl md:text-2xl mb-8 text-gray-200">
                {slide.subtitle}
              </p>
            </div>
          </div>
        ))}
        <div className="absolute inset-x-0 bottom-10 flex flex-col items-center">
          <a
            href="https://wa.me/+6281234567890"
            className="bg-gradient-to-r from-green-400 to-emerald-600 text-white px-8 py-4 rounded-full text-lg font-semibold transition-all transform hover:scale-105 hover:shadow-[0_0_30px_rgba(52,211,153,0.5)] flex items-center gap-2"
          >
            <MessageCircle className="w-5 h-5" />
            Gas Chat WhatsApp!
          </a>
        </div>
      </div>
     </div>

      {/* About Section */}
      <section className="py-20 px-4">
        <div className="max-w-4xl mx-auto text-center">
          <div className="inline-block mb-8">
            <Lock className="w-12 h-12 text-green-400 animate-bounce" />
          </div>
          <h2 className="text-4xl font-bold mb-8 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
            About Us
          </h2>
          <p className="text-xl text-gray-300 leading-relaxed">
            Kita tuh spesialis duplikasi kunci yang udah trusted banget! 
            Handle berbagai jenis kunci dari rumah, motor, sampe mobil. 
            Panggilan ready, harga friendly, dan dijamin hasil premium! 💯
          </p>
        </div>
      </section>

      {/* Benefits Section */}
      <section className="py-20 px-4 relative overflow-hidden">
        <div className="absolute inset-0 bg-gradient-to-b from-green-900/20 to-transparent" />
        <div className="max-w-6xl mx-auto relative">
          <h2 className="text-4xl font-bold text-center mb-12 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
            Why Choose Us?
          </h2>
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
            {benefits.map((benefit, index) => (
              <div 
                key={index}
                className="bg-gradient-to-br from-gray-900 to-gray-800 p-6 rounded-2xl text-center transform transition-all hover:scale-105 hover:shadow-[0_0_30px_rgba(52,211,153,0.2)]"
              >
                <benefit.icon className="w-12 h-12 mx-auto mb-4 text-green-400" />
                <h3 className="text-xl font-semibold mb-2">{benefit.title}</h3>
                <p className="text-gray-400">{benefit.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Testimonials */}
      <section className="py-20 px-4 bg-gradient-to-b from-black to-gray-900">
        <div className="max-w-4xl mx-auto">
          <h2 className="text-4xl font-bold text-center mb-12 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
            Reviews Customers
          </h2>
          <div className="relative h-64">
            {testimonials.map((testimonial, index) => (
              <div
                key={index}
                className={`absolute w-full transition-all duration-500 transform ${
                  index === currentTestimonial
                    ? 'opacity-100 translate-x-0'
                    : 'opacity-0 translate-x-full'
                }`}
              >
                <div className="bg-gradient-to-br from-gray-900 to-gray-800 p-8 rounded-2xl text-center">
                  <p className="text-xl mb-4">"{testimonial.text}"</p>
                  <p className="font-semibold text-green-400">{testimonial.name}</p>
                  <p className="text-sm text-gray-400 mb-2">{testimonial.tag}</p>
                  <div className="flex justify-center mt-2">
                    {[...Array(testimonial.rating)].map((_, i) => (
                      <Star key={i} className="w-5 h-5 text-yellow-400 fill-current" />
                    ))}
                  </div>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* FAQ Section */}
      <section className="py-20 px-4">
        <div className="max-w-3xl mx-auto">
          <h2 className="text-4xl font-bold text-center mb-12 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
            FAQ
          </h2>
          <div className="space-y-4">
            {faqs.map((faq, index) => (
              <div
                key={index}
                className="bg-gradient-to-br from-gray-900 to-gray-800 rounded-2xl overflow-hidden transition-all hover:shadow-[0_0_30px_rgba(52,211,153,0.1)]"
              >
                <button
                  className="w-full px-6 py-4 text-left flex justify-between items-center"
                  onClick={() => setOpenFaq(openFaq === index ? null : index)}
                >
                  <span className="font-semibold">{faq.question}</span>
                  <ChevronDown
                    className={`w-5 h-5 transform transition-transform text-green-400 ${
                      openFaq === index ? 'rotate-180' : ''
                    }`}
                  />
                </button>
                <div
                  className={`px-6 transition-all duration-300 ${
                    openFaq === index ? 'py-4' : 'py-0 h-0'
                  }`}
                >
                  <p className="text-gray-300">{faq.answer}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Location Section */}
      <section className="py-20 px-4 bg-gradient-to-b from-gray-900 to-black">
        <div className="max-w-6xl mx-auto">
          <h2 className="text-4xl font-bold text-center mb-12 bg-clip-text text-transparent bg-gradient-to-r from-green-400 to-emerald-600">
            Lokasi Kami
          </h2>
          <div className="aspect-w-16 aspect-h-9 rounded-2xl overflow-hidden shadow-[0_0_30px_rgba(52,211,153,0.2)]">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.757310872387!2d106.9376817!3d-6.3234155!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e699300248389c5%3A0x4098febce6b5b9ab!2sDUPLIKAT%20KUNCI!5e0!3m2!1sen!2sid!4v1712952700403!5m2!1sen!2sid"
              width="100%"
              height="450"
              style={{ border: 0 }}
              allowFullScreen
              loading="lazy"
              className="rounded-2xl"
            ></iframe>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="py-12 px-4">
        <div className="max-w-6xl mx-auto text-center">
          <div className="flex justify-center space-x-6 mb-8">
            <a href="tel:+6285814766454" className="hover:text-green-400 transition-colors">
              <Phone className="w-6 h-6" />
            </a>
            <a href="https://wa.me/+6285814766454" className="hover:text-green-400 transition-colors">
              <MessageCircle className="w-6 h-6" />
            </a>
            <a href="https://maps.app.goo.gl/e5af6PMGS3TNFBbH6" className="hover:text-green-400 transition-colors">
              <MapPin className="w-6 h-6" />
            </a>
          </div>
          <p className="text-gray-400">
            © 2025 AR Duplikat Kunci • All rights reserved • Made with 💚
          </p>
        </div>
      </footer>
      </div>
  );
}

export default App;