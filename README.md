export default function MNhatStore() { const products = [ { title: "Acc Blox Fruit Max", price: "199K", desc: "Max level • V4 • CDK • Soul Guitar" }, { title: "Cloud Phone VIP", price: "99K/tháng", desc: "Treo game 24/7 • FPS ổn định" }, { title: "Script Premium", price: "49K", desc: "Auto Farm • Auto Raid • Update mới" } ];

return ( <div className="min-h-screen bg-white text-slate-900"> {/* Header */} <header className="border-b border-slate-200 bg-white sticky top-0 z-50"> <div className="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between"> <div> <h1 className="text-3xl font-bold text-cyan-500">M.NhatStore</h1> <p className="text-sm text-slate-500">Blox Fruit • Cloud Phone • Script</p> </div>

<nav className="hidden md:flex gap-6 text-sm font-medium">
        <a href="#home" className="hover:text-cyan-500">Trang Chủ</a>
        <a href="#products" className="hover:text-cyan-500">Sản Phẩm</a>
        <a href="#cloud" className="hover:text-cyan-500">Cloud Phone</a>
        <a href="#feedback" className="hover:text-cyan-500">Feedback</a>
        <a href="#contact" className="hover:text-cyan-500">Liên Hệ</a>
      </nav>

      <button className="bg-cyan-400 hover:bg-cyan-500 text-white px-5 py-2 rounded-2xl shadow-lg">
        Đăng Nhập
      </button>
    </div>
  </header>

  {/* Hero */}
  <section id="home" className="max-w-7xl mx-auto px-6 py-20 grid md:grid-cols-2 gap-12 items-center">
    <div>
      <div className="inline-block px-4 py-1 rounded-full bg-cyan-100 text-cyan-600 text-sm mb-5">
        Shop Uy Tín 2026
      </div>

      <h2 className="text-5xl font-extrabold leading-tight mb-6">
        Shop Acc Blox Fruit & Cloud Phone Chuyên Nghiệp
      </h2>

      <p className="text-slate-600 text-lg mb-8">
        Mua acc nhanh • Nạp tiền tự động • Hỗ trợ 24/7 • Giao dịch an toàn.
      </p>

      <div className="flex gap-4 flex-wrap">
        <button className="bg-cyan-500 hover:bg-cyan-600 text-white px-6 py-3 rounded-2xl shadow-lg">
          Mua Acc
        </button>

        <button className="border border-cyan-400 text-cyan-500 px-6 py-3 rounded-2xl hover:bg-cyan-50">
          Thuê Cloud Phone
        </button>
      </div>
    </div>

    <div className="bg-gradient-to-br from-cyan-100 to-white rounded-3xl p-8 shadow-2xl border border-cyan-100">
      <div className="grid gap-5">
        <div className="bg-white rounded-2xl p-5 shadow-md">
          <h3 className="font-bold text-lg mb-2">Tự Động 100%</h3>
          <p className="text-slate-500">Nạp tiền và nhận acc tự động.</p>
        </div>

        <div className="bg-white rounded-2xl p-5 shadow-md">
          <h3 className="font-bold text-lg mb-2">Cloud Phone VIP</h3>
          <p className="text-slate-500">Treo game mượt • Online 24/24.</p>
        </div>

        <div className="bg-white rounded-2xl p-5 shadow-md">
          <h3 className="font-bold text-lg mb-2">Support 24/7</h3>
          <p className="text-slate-500">Discord • Facebook • Zalo.</p>
        </div>
      </div>
    </div>
  </section>

  {/* Products */}
  <section id="products" className="bg-slate-50 py-20">
    <div className="max-w-7xl mx-auto px-6">
      <div className="text-center mb-14">
        <h2 className="text-4xl font-bold mb-3">Sản Phẩm Nổi Bật</h2>
        <p className="text-slate-500">Acc • Cloud • Script • Dịch vụ</p>
      </div>

      <div className="grid md:grid-cols-3 gap-8">
        {products.map((item, index) => (
          <div
            key={index}
            className="bg-white rounded-3xl shadow-lg p-7 border border-slate-100 hover:-translate-y-2 transition-all"
          >
            <div className="w-14 h-14 rounded-2xl bg-cyan-100 mb-5"></div>

            <h3 className="text-2xl font-bold mb-2">{item.title}</h3>

            <p className="text-slate-500 mb-5">{item.desc}</p>

            <div className="text-3xl font-extrabold text-cyan-500 mb-6">
              {item.price}
            </div>

            <button className="w-full bg-cyan-500 hover:bg-cyan-600 text-white py-3 rounded-2xl">
              Mua Ngay
            </button>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Features */}
  <section id="cloud" className="py-20">
    <div className="max-w-7xl mx-auto px-6 grid md:grid-cols-2 gap-10 items-center">
      <div>
        <h2 className="text-4xl font-bold mb-5">
          Cloud Phone Treo Game 24/7
        </h2>

        <p className="text-slate-600 text-lg mb-8">
          Hỗ trợ treo game ổn định, online liên tục và tối ưu cho Blox Fruit.
        </p>

        <div className="grid gap-4">
          <div className="bg-cyan-50 p-5 rounded-2xl">
            ⚡ Ping ổn định
          </div>

          <div className="bg-cyan-50 p-5 rounded-2xl">
            ⚡ FPS tối ưu
          </div>

          <div className="bg-cyan-50 p-5 rounded-2xl">
            ⚡ Support nhanh
          </div>
        </div>
      </div>

      <div className="bg-gradient-to-br from-cyan-400 to-cyan-200 rounded-3xl h-[420px] shadow-2xl"></div>
    </div>
  </section>

  {/* Feedback */}
  <section id="feedback" className="bg-slate-50 py-20">
    <div className="max-w-7xl mx-auto px-6 text-center">
      <h2 className="text-4xl font-bold mb-12">Feedback Khách Hàng</h2>

      <div className="grid md:grid-cols-3 gap-8">
        {[1, 2, 3].map((item) => (
          <div
            key={item}
            className="bg-white rounded-3xl p-7 shadow-lg"
          >
            <div className="text-5xl mb-4">⭐</div>
            <p className="text-slate-600 mb-5">
              Shop giao acc nhanh, support nhiệt tình và cloud phone rất ổn định.
            </p>
            <h4 className="font-bold">Khách Hàng #{item}</h4>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Contact */}
  <section id="contact" className="py-20">
    <div className="max-w-5xl mx-auto px-6 text-center">
      <h2 className="text-4xl font-bold mb-5">Liên Hệ Hỗ Trợ</h2>

      <p className="text-slate-500 text-lg mb-10">
        Hỗ trợ qua Facebook, Discord và Zalo 24/7.
      </p>

      <div className="flex flex-wrap justify-center gap-5">
        <button className="bg-cyan-500 text-white px-8 py-4 rounded-2xl shadow-lg hover:bg-cyan-600">
          Facebook
        </button>

        <button className="border border-cyan-400 text-cyan-500 px-8 py-4 rounded-2xl hover:bg-cyan-50">
          Discord
        </button>

        <button className="border border-cyan-400 text-cyan-500 px-8 py-4 rounded-2xl hover:bg-cyan-50">
          Zalo
        </button>
      </div>
    </div>
  </section>

  {/* Footer */}
  <footer className="border-t border-slate-200 py-8 text-center text-slate-500">
    © 2026 M.NhatStore — All Rights Reserved
  </footer>
</div>

); }
