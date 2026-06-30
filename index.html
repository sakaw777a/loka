import React, { useState, useMemo, useEffect } from "react";
import {
  Sparkles,
  CalendarClock,
  ClipboardList,
  ChevronDown,
  ChevronRight,
  RotateCcw,
  Check,
  ArrowRight,
  ShieldCheck,
  AlertTriangle,
  Droplet,
  Wind,
  Layers,
  ShieldAlert,
  CalendarDays,
} from "lucide-react";

/* ============================================================================
   SAKAW BEAUTYTOOLS — mock data
   ============================================================================ */

const SWATCH_COLORS = {
  "Fair-Cool": "#F3DCD6",
  "Fair-Warm": "#F5DCC0",
  "Fair-Neutral": "#F2DACB",
  "Light-Cool": "#EAC3B9",
  "Light-Warm": "#EAC79C",
  "Light-Neutral": "#E8C5A9",
  "Medium-Cool": "#CB9C8E",
  "Medium-Warm": "#D2A06C",
  "Medium-Neutral": "#CE9C77",
  "Tan-Cool": "#AD7868",
  "Tan-Warm": "#B97D4C",
  "Tan-Neutral": "#B27A56",
  "Deep-Cool": "#7C4F45",
  "Deep-Warm": "#8C5530",
  "Deep-Neutral": "#82512E",
};

function swatchColor(depth, undertone) {
  return SWATCH_COLORS[`${depth}-${undertone}`] || "#D8C3B5";
}

const BRANDS = [
  {
    id: "mac",
    name: "MAC",
    initials: "MAC",
    products: [
      {
        id: "mac-studiofix",
        name: "Studio Fix Fluid SPF15",
        type: "Liquid Foundation",
        shades: [
          { code: "NC10", depth: "Fair", undertone: "Cool" },
          { code: "NC15", depth: "Fair", undertone: "Neutral" },
          { code: "NW15", depth: "Fair", undertone: "Warm" },
          { code: "NC20", depth: "Light", undertone: "Cool" },
          { code: "NC25", depth: "Light", undertone: "Neutral" },
          { code: "NW25", depth: "Light", undertone: "Warm" },
          { code: "NC30", depth: "Medium", undertone: "Cool" },
          { code: "NC35", depth: "Medium", undertone: "Neutral" },
          { code: "NW35", depth: "Medium", undertone: "Warm" },
          { code: "NC40", depth: "Tan", undertone: "Cool" },
          { code: "NC42", depth: "Tan", undertone: "Neutral" },
          { code: "NW43", depth: "Tan", undertone: "Warm" },
          { code: "NC45", depth: "Deep", undertone: "Cool" },
          { code: "NC50", depth: "Deep", undertone: "Neutral" },
          { code: "NW47", depth: "Deep", undertone: "Warm" },
        ],
      },
      {
        id: "mac-radiance",
        name: "Studio Radiance Serum-Powered Foundation",
        type: "Liquid Foundation",
        shades: [
          { code: "NC15", depth: "Fair", undertone: "Neutral" },
          { code: "NW20", depth: "Light", undertone: "Warm" },
          { code: "NC30", depth: "Medium", undertone: "Cool" },
          { code: "NW35", depth: "Medium", undertone: "Warm" },
          { code: "NC42", depth: "Tan", undertone: "Neutral" },
          { code: "NW45", depth: "Deep", undertone: "Warm" },
        ],
      },
    ],
  },
  {
    id: "maybelline",
    name: "Maybelline",
    initials: "MNY",
    products: [
      {
        id: "mny-fitme",
        name: "Fit Me Matte + Poreless",
        type: "Liquid Foundation",
        shades: [
          { code: "112", depth: "Fair", undertone: "Cool" },
          { code: "105", depth: "Fair", undertone: "Neutral" },
          { code: "110", depth: "Fair", undertone: "Warm" },
          { code: "115", depth: "Light", undertone: "Cool" },
          { code: "120", depth: "Light", undertone: "Neutral" },
          { code: "128", depth: "Light", undertone: "Warm" },
          { code: "235", depth: "Medium", undertone: "Cool" },
          { code: "220", depth: "Medium", undertone: "Neutral" },
          { code: "228", depth: "Medium", undertone: "Warm" },
          { code: "320", depth: "Tan", undertone: "Cool" },
          { code: "310", depth: "Tan", undertone: "Neutral" },
          { code: "330", depth: "Tan", undertone: "Warm" },
          { code: "370", depth: "Deep", undertone: "Cool" },
          { code: "355", depth: "Deep", undertone: "Neutral" },
          { code: "360", depth: "Deep", undertone: "Warm" },
        ],
      },
      {
        id: "mny-superstay",
        name: "Super Stay Full Coverage",
        type: "Liquid Foundation",
        shades: [
          { code: "102", depth: "Fair", undertone: "Neutral" },
          { code: "128", depth: "Light", undertone: "Warm" },
          { code: "220", depth: "Medium", undertone: "Neutral" },
          { code: "232", depth: "Medium", undertone: "Warm" },
          { code: "322", depth: "Tan", undertone: "Cool" },
          { code: "362", depth: "Deep", undertone: "Warm" },
        ],
      },
    ],
  },
  {
    id: "fenty",
    name: "Fenty Beauty",
    initials: "FB",
    products: [
      {
        id: "fenty-profiltr",
        name: "Pro Filt'r Soft Matte",
        type: "Liquid Foundation",
        shades: [
          { code: "130", depth: "Fair", undertone: "Cool" },
          { code: "100", depth: "Fair", undertone: "Neutral" },
          { code: "110", depth: "Fair", undertone: "Warm" },
          { code: "160", depth: "Light", undertone: "Cool" },
          { code: "170", depth: "Light", undertone: "Neutral" },
          { code: "180", depth: "Light", undertone: "Warm" },
          { code: "230", depth: "Medium", undertone: "Cool" },
          { code: "240", depth: "Medium", undertone: "Neutral" },
          { code: "250", depth: "Medium", undertone: "Warm" },
          { code: "310", depth: "Tan", undertone: "Cool" },
          { code: "330", depth: "Tan", undertone: "Neutral" },
          { code: "340", depth: "Tan", undertone: "Warm" },
          { code: "420", depth: "Deep", undertone: "Cool" },
          { code: "440", depth: "Deep", undertone: "Neutral" },
          { code: "450", depth: "Deep", undertone: "Warm" },
        ],
      },
      {
        id: "fenty-eaze",
        name: "Eaze Drop Blurring Skin Tint",
        type: "Skin Tint",
        shades: [
          { code: "100", depth: "Fair", undertone: "Neutral" },
          { code: "180", depth: "Light", undertone: "Warm" },
          { code: "240", depth: "Medium", undertone: "Neutral" },
          { code: "230", depth: "Medium", undertone: "Cool" },
          { code: "330", depth: "Tan", undertone: "Neutral" },
          { code: "440", depth: "Deep", undertone: "Neutral" },
        ],
      },
    ],
  },
  {
    id: "estee",
    name: "Estée Lauder",
    initials: "EL",
    products: [
      {
        id: "el-doublewear",
        name: "Double Wear Stay-in-Place",
        type: "Liquid Foundation",
        shades: [
          { code: "1C0 Shell", depth: "Fair", undertone: "Cool" },
          { code: "1N1 Ivory Nude", depth: "Fair", undertone: "Neutral" },
          { code: "1W1 Bone", depth: "Fair", undertone: "Warm" },
          { code: "2C2 Pale Almond", depth: "Light", undertone: "Cool" },
          { code: "2N1 Desert Beige", depth: "Light", undertone: "Neutral" },
          { code: "2W1 Dawn", depth: "Light", undertone: "Warm" },
          { code: "3C2 Pebble", depth: "Medium", undertone: "Cool" },
          { code: "3N1 Dusk", depth: "Medium", undertone: "Neutral" },
          { code: "3W1 Tawny", depth: "Medium", undertone: "Warm" },
          { code: "4C2 Auburn", depth: "Tan", undertone: "Cool" },
          { code: "4N1 Shell Beige", depth: "Tan", undertone: "Neutral" },
          { code: "4W1 Honey Bronze", depth: "Tan", undertone: "Warm" },
          { code: "5C1 Rich Cocoa", depth: "Deep", undertone: "Cool" },
          { code: "5N1 Cinnamon", depth: "Deep", undertone: "Neutral" },
          { code: "5W1 Truffle", depth: "Deep", undertone: "Warm" },
        ],
      },
      {
        id: "el-futurist",
        name: "Futurist Hydra Rescue SPF45",
        type: "Liquid Foundation",
        shades: [
          { code: "1N1 Ivory Nude", depth: "Fair", undertone: "Neutral" },
          { code: "2W1 Dawn", depth: "Light", undertone: "Warm" },
          { code: "3N1 Dusk", depth: "Medium", undertone: "Neutral" },
          { code: "3C2 Pebble", depth: "Medium", undertone: "Cool" },
          { code: "4W1 Honey Bronze", depth: "Tan", undertone: "Warm" },
          { code: "5N1 Cinnamon", depth: "Deep", undertone: "Neutral" },
        ],
      },
    ],
  },
  {
    id: "loreal",
    name: "L'Oréal Paris",
    initials: "LP",
    products: [
      {
        id: "loreal-truematch",
        name: "True Match Liquid Foundation",
        type: "Liquid Foundation",
        shades: [
          { code: "1C Fair", depth: "Fair", undertone: "Cool" },
          { code: "1N Fair", depth: "Fair", undertone: "Neutral" },
          { code: "1W Fair", depth: "Fair", undertone: "Warm" },
          { code: "3C Light", depth: "Light", undertone: "Cool" },
          { code: "3N Light", depth: "Light", undertone: "Neutral" },
          { code: "3W Light", depth: "Light", undertone: "Warm" },
          { code: "5C Medium", depth: "Medium", undertone: "Cool" },
          { code: "5N Medium", depth: "Medium", undertone: "Neutral" },
          { code: "5W Medium", depth: "Medium", undertone: "Warm" },
          { code: "7C Tan", depth: "Tan", undertone: "Cool" },
          { code: "7N Tan", depth: "Tan", undertone: "Neutral" },
          { code: "7W Tan", depth: "Tan", undertone: "Warm" },
          { code: "9C Deep", depth: "Deep", undertone: "Cool" },
          { code: "9N Deep", depth: "Deep", undertone: "Neutral" },
          { code: "9W Deep", depth: "Deep", undertone: "Warm" },
        ],
      },
      {
        id: "loreal-infallible",
        name: "Infallible 24H Fresh Wear",
        type: "Liquid Foundation",
        shades: [
          { code: "1N Fair", depth: "Fair", undertone: "Neutral" },
          { code: "3W Light", depth: "Light", undertone: "Warm" },
          { code: "5N Medium", depth: "Medium", undertone: "Neutral" },
          { code: "5C Medium", depth: "Medium", undertone: "Cool" },
          { code: "7W Tan", depth: "Tan", undertone: "Warm" },
          { code: "9N Deep", depth: "Deep", undertone: "Neutral" },
        ],
      },
    ],
  },
];

const PAO_CONFIG = [
  { id: "mascara", label: "Mascara", months: 3 },
  { id: "foundation", label: "Foundation", months: 12 },
  { id: "lipstick", label: "Lipstick", months: 24 },
  { id: "skincare", label: "Skincare Liquid", months: 6 },
  { id: "powder", label: "Powder", months: 24 },
];

const QUIZ_QUESTIONS = [
  {
    id: "shine",
    question: "By the middle of the afternoon, how does your face look?",
    options: [
      { text: "Shiny all over, especially across the T-zone", type: "Oily" },
      { text: "Tight and matte, with no shine anywhere", type: "Dry" },
      { text: "Shiny on the T-zone, but normal on the cheeks", type: "Combination" },
      { text: "Fine, but a little red or irritated-looking", type: "Sensitive" },
    ],
  },
  {
    id: "pores",
    question: "How would you describe your pores?",
    options: [
      { text: "Large and clearly visible, especially on the nose", type: "Oily" },
      { text: "Very fine — almost impossible to spot", type: "Dry" },
      { text: "Visible on the nose and forehead, small on the cheeks", type: "Combination" },
      { text: "Visible but the surrounding skin reacts easily", type: "Sensitive" },
    ],
  },
  {
    id: "flaking",
    question: "Does your skin ever flake or feel rough to the touch?",
    options: [
      { text: "Rarely — if anything, it feels slick", type: "Oily" },
      { text: "Often, especially around the nose and cheeks", type: "Dry" },
      { text: "Only on the cheeks, never on the T-zone", type: "Combination" },
      { text: "Sometimes, usually paired with stinging or redness", type: "Sensitive" },
    ],
  },
  {
    id: "reaction",
    question: "When you try a brand-new skincare or makeup formula, what usually happens?",
    options: [
      { text: "It breaks me out or feels heavy by midday", type: "Oily" },
      { text: "No issues at all, even with rich, heavy formulas", type: "Dry" },
      { text: "It depends entirely on the area of my face", type: "Combination" },
      { text: "It often stings, itches, or turns my skin red", type: "Sensitive" },
    ],
  },
];

const SKIN_PROFILES = {
  Oily: {
    title: "Oily",
    icon: Droplet,
    description:
      "Your skin produces extra sebum, which keeps it resilient and slow to wrinkle, but prone to shine and clogged pores throughout the day.",
    tips: [
      "Blot shine midday instead of layering on more powder.",
      "Prime with a mattifying, pore-minimizing primer before foundation.",
      "Skip heavy, balm-based creams — they sit on top of natural oil.",
      "Use clay or charcoal masks weekly to keep pores clear.",
    ],
    textures: ["Matte finish", "Oil-control formulas", "Lightweight fluids", "Oil-free SPF"],
  },
  Dry: {
    title: "Dry",
    icon: Wind,
    description:
      "Your skin produces less natural oil, leaving it prone to tightness and flaking, but it's also less likely to show shine or breakouts.",
    tips: [
      "Hydrate with a rich moisturizer a few minutes before foundation.",
      "Avoid powder-heavy products — they emphasize dry patches.",
      "Finish with a hydrating setting mist instead of powder.",
      "Look for hyaluronic acid and ceramides in your skincare.",
    ],
    textures: ["Dewy, luminous finish", "Hydrating cream formulas", "Balm-based products", "Glow-enhancing primers"],
  },
  Combination: {
    title: "Combination",
    icon: Layers,
    description:
      "Your T-zone behaves differently from your cheeks — typically oilier down the center and drier or more balanced at the edges.",
    tips: [
      "Apply mattifying primer only on the T-zone.",
      "Hydrate the cheeks separately with a richer layer of moisturizer.",
      "Blot midday, but only where shine actually appears.",
      "Choose a foundation that's buildable rather than one-finish-fits-all.",
    ],
    textures: ["Satin, balanced finish", "Multi-zone application formulas", "Buildable medium coverage", "Lightweight gel-creams"],
  },
  Sensitive: {
    title: "Sensitive",
    icon: ShieldAlert,
    description:
      "Your skin reacts visibly to new ingredients, environmental changes, or friction — with redness, stinging, or irritation more often than oiliness or dryness.",
    tips: [
      "Patch test every new formula on your inner arm for 24 hours first.",
      "Choose fragrance-free and dye-free formulations whenever possible.",
      "Look for soothing ingredients like centella asiatica, oat, or panthenol.",
      "Introduce one new product at a time, never several at once.",
    ],
    textures: ["Hypoallergenic formulas", "Fragrance-free bases", "Mineral & gentle pigments", "Barrier-supporting textures"],
  },
};

const TABS = [
  { id: "shade", label: "Shade Finder", icon: Sparkles },
  { id: "pao", label: "PAO Calculator", icon: CalendarClock },
  { id: "quiz", label: "Skin Quiz", icon: ClipboardList },
];

/* ============================================================================
   Small shared pieces
   ============================================================================ */

function ShadeMark({ size = 40 }) {
  return (
    <svg width={size} height={size} viewBox="0 0 48 48" className="shrink-0" aria-hidden="true">
      <circle cx="18" cy="20" r="14" fill="#F3D6DE" opacity="0.95" />
      <circle cx="30" cy="18" r="12" fill="#E8B9C6" opacity="0.92" />
      <circle cx="24" cy="30" r="13" fill="#B76E79" opacity="0.88" />
    </svg>
  );
}

function AdSlot({ label = "Advertisement", variant = "banner" }) {
  const heightClass =
    variant === "sidebar" ? "h-64" : variant === "inline" ? "h-20" : "h-20 md:h-24";
  return (
    <div className={`sakaw-ad-slot w-full ${heightClass} rounded-2xl flex flex-col items-center justify-center gap-1 px-4`}>
      <span className="sakaw-ad-label">{label}</span>
      <span className="sakaw-ad-sub">Google AdSense Placeholder</span>
    </div>
  );
}

function SectionEyebrow({ children }) {
  return <span className="sakaw-eyebrow">{children}</span>;
}

/* ============================================================================
   TOOL 1 — Foundation Shade Finder
   ============================================================================ */

function ShadeFinder() {
  const [brandId, setBrandId] = useState(null);
  const [productId, setProductId] = useState(null);
  const [shadeCode, setShadeCode] = useState(null);

  const selectedBrand = BRANDS.find((b) => b.id === brandId) || null;
  const selectedProduct = selectedBrand?.products.find((p) => p.id === productId) || null;
  const selectedShade = selectedProduct?.shades.find((s) => s.code === shadeCode) || null;

  const matches = useMemo(() => {
    if (!selectedShade || !selectedBrand) return [];
    const results = [];
    BRANDS.forEach((brand) => {
      if (brand.id === selectedBrand.id) return;
      brand.products.forEach((product) => {
        product.shades.forEach((shade) => {
          if (shade.depth === selectedShade.depth && shade.undertone === selectedShade.undertone) {
            const sameType = selectedProduct && product.type === selectedProduct.type;
            results.push({
              brand,
              product,
              shade,
              match: sameType ? 100 : 97,
            });
          }
        });
      });
    });
    return results.sort((a, b) => b.match - a.match || a.brand.name.localeCompare(b.brand.name));
  }, [selectedShade, selectedBrand, selectedProduct]);

  function reset() {
    setBrandId(null);
    setProductId(null);
    setShadeCode(null);
  }

  const step = !brandId ? 1 : !productId ? 2 : !shadeCode ? 3 : 4;

  return (
    <div className="sakaw-fade-in">
      <div className="flex items-start justify-between gap-4 flex-wrap mb-6">
        <div>
          <SectionEyebrow>Foundation Shade Finder · by Sakaw</SectionEyebrow>
          <h2 className="sakaw-h2 mt-1">Find your shade in any brand</h2>
          <p className="sakaw-body-soft mt-2 max-w-xl">
            Choose your current brand, product, and shade. The Sakaw Algorithm cross-references
            skin depth and undertone to surface equivalent shades across every other brand in our library.
          </p>
        </div>
        {step > 1 && (
          <button onClick={reset} className="sakaw-btn-ghost shrink-0">
            <RotateCcw size={15} />
            Start over
          </button>
        )}
      </div>

      {/* Step indicator */}
      <div className="flex items-center gap-2 mb-8 flex-wrap">
        {["Brand", "Product", "Shade"].map((label, i) => {
          const n = i + 1;
          const active = step === n;
          const done = step > n;
          return (
            <div key={label} className="flex items-center gap-2">
              <div className={`sakaw-step-dot ${active ? "sakaw-step-active" : ""} ${done ? "sakaw-step-done" : ""}`}>
                {done ? <Check size={13} /> : n}
              </div>
              <span className={`sakaw-step-label ${active ? "sakaw-step-label-active" : ""}`}>{label}</span>
              {n < 3 && <ChevronRight size={15} className="sakaw-step-chevron" />}
            </div>
          );
        })}
      </div>

      {/* Step 1: Brand */}
      <div className="sakaw-glass rounded-3xl p-5 md:p-7 mb-5">
        <h3 className="sakaw-h4 mb-4">1. Select your current brand</h3>
        <div className="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-3">
          {BRANDS.map((brand) => (
            <button
              key={brand.id}
              onClick={() => {
                setBrandId(brand.id);
                setProductId(null);
                setShadeCode(null);
              }}
              className={`sakaw-option-card ${brandId === brand.id ? "sakaw-option-card-active" : ""}`}
            >
              <span className="sakaw-monogram">{brand.initials}</span>
              <span className="sakaw-option-label">{brand.name}</span>
            </button>
          ))}
        </div>
      </div>

      {/* Step 2: Product */}
      {selectedBrand && (
        <div className="sakaw-glass rounded-3xl p-5 md:p-7 mb-5 sakaw-fade-in">
          <h3 className="sakaw-h4 mb-4">2. Select the product</h3>
          <div className="grid grid-cols-1 sm:grid-cols-2 gap-3">
            {selectedBrand.products.map((product) => (
              <button
                key={product.id}
                onClick={() => {
                  setProductId(product.id);
                  setShadeCode(null);
                }}
                className={`sakaw-option-card sakaw-option-card-wide ${productId === product.id ? "sakaw-option-card-active" : ""}`}
              >
                <span className="sakaw-option-label-lg">{product.name}</span>
                <span className="sakaw-option-tag">{product.type} · {product.shades.length} shades</span>
              </button>
            ))}
          </div>
        </div>
      )}

      {/* Step 3: Shade */}
      {selectedProduct && (
        <div className="sakaw-glass rounded-3xl p-5 md:p-7 mb-5 sakaw-fade-in">
          <h3 className="sakaw-h4 mb-4">3. Select your current shade</h3>
          <div className="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-3">
            {selectedProduct.shades.map((shade) => (
              <button
                key={shade.code}
                onClick={() => setShadeCode(shade.code)}
                className={`sakaw-shade-card ${shadeCode === shade.code ? "sakaw-shade-card-active" : ""}`}
              >
                <span className="sakaw-shade-dot" style={{ background: swatchColor(shade.depth, shade.undertone) }} />
                <span className="sakaw-shade-code">{shade.code}</span>
                <span className="sakaw-shade-meta">{shade.depth} · {shade.undertone}</span>
              </button>
            ))}
          </div>
        </div>
      )}

      {/* Results */}
      {selectedShade && (
        <div className="sakaw-fade-in">
          <div className="sakaw-glass-strong rounded-3xl p-5 md:p-7 mb-6 flex items-center gap-5 flex-wrap">
            <span className="sakaw-shade-dot-lg" style={{ background: swatchColor(selectedShade.depth, selectedShade.undertone) }} />
            <div>
              <p className="sakaw-eyebrow">Your profile</p>
              <p className="sakaw-h4 mt-1">
                {selectedBrand.name} {selectedProduct.name} — {selectedShade.code}
              </p>
              <p className="sakaw-body-soft mt-1">
                Skin depth <strong className="sakaw-strong">{selectedShade.depth}</strong> · Undertone{" "}
                <strong className="sakaw-strong">{selectedShade.undertone}</strong>
              </p>
            </div>
          </div>

          <h3 className="sakaw-h4 mb-4">Matching shades across other brands</h3>

          {matches.length === 0 ? (
            <p className="sakaw-body-soft">No equivalent shades found in the current library yet.</p>
          ) : (
            <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 mb-6">
              {matches.map((m, idx) => (
                <div key={`${m.brand.id}-${m.product.id}-${m.shade.code}`} className="sakaw-result-card sakaw-fade-in" style={{ animationDelay: `${idx * 60}ms` }}>
                  <div className="flex items-center justify-between mb-3">
                    <span className="sakaw-monogram sakaw-monogram-sm">{m.brand.initials}</span>
                    <span className="sakaw-match-badge">
                      <Sparkles size={12} />
                      {m.match}% Match by Sakaw Algorithm
                    </span>
                  </div>
                  <span className="sakaw-shade-dot-lg block mb-3" style={{ background: swatchColor(m.shade.depth, m.shade.undertone) }} />
                  <p className="sakaw-result-brand">{m.brand.name}</p>
                  <p className="sakaw-result-product">{m.product.name}</p>
                  <p className="sakaw-result-shade">Shade {m.shade.code}</p>
                  <p className="sakaw-option-tag mt-1">{m.shade.depth} · {m.shade.undertone}</p>
                </div>
              ))}
            </div>
          )}

          <AdSlot label="Advertisement" variant="inline" />
        </div>
      )}
    </div>
  );
}

/* ============================================================================
   TOOL 2 — Cosmetic PAO Calculator
   ============================================================================ */

function daysBetween(a, b) {
  const msPerDay = 86400000;
  const da = new Date(a.getFullYear(), a.getMonth(), a.getDate());
  const db = new Date(b.getFullYear(), b.getMonth(), b.getDate());
  return Math.round((db - da) / msPerDay);
}

function addMonths(date, months) {
  const d = new Date(date);
  d.setMonth(d.getMonth() + months);
  return d;
}

function formatDate(d) {
  return d.toLocaleDateString(undefined, { year: "numeric", month: "short", day: "numeric" });
}

function PaoCalculator() {
  const [categoryId, setCategoryId] = useState("foundation");
  const [dateOpened, setDateOpened] = useState("");

  const category = PAO_CONFIG.find((c) => c.id === categoryId);

  const result = useMemo(() => {
    if (!dateOpened) return null;
    const opened = new Date(dateOpened + "T00:00:00");
    if (isNaN(opened.getTime())) return null;
    const expiration = addMonths(opened, category.months);
    const today = new Date();
    const totalDays = daysBetween(opened, expiration);
    const elapsedDays = daysBetween(opened, today);
    const remainingDays = totalDays - elapsedDays;
    const isExpired = remainingDays <= 0;
    const percentRemaining = Math.max(0, Math.min(100, (remainingDays / totalDays) * 100));
    return { opened, expiration, totalDays, remainingDays, isExpired, percentRemaining };
  }, [dateOpened, category]);

  const radius = 76;
  const circumference = 2 * Math.PI * radius;
  const pct = result ? result.percentRemaining : 100;
  const dashoffset = circumference * (1 - pct / 100);

  return (
    <div className="sakaw-fade-in">
      <SectionEyebrow>Cosmetic PAO Calculator</SectionEyebrow>
      <h2 className="sakaw-h2 mt-1">When does it actually expire?</h2>
      <p className="sakaw-body-soft mt-2 max-w-xl mb-6">
        Select your product category and the date you opened it. Sakaw calculates the Period After
        Opening and tells you exactly how much safe wear time remains.
      </p>

      <div className="sakaw-glass rounded-3xl p-5 md:p-7 mb-6">
        <div className="grid grid-cols-1 md:grid-cols-2 gap-5">
          <div>
            <label className="sakaw-label">Product category</label>
            <div className="relative mt-2">
              <select
                value={categoryId}
                onChange={(e) => setCategoryId(e.target.value)}
                className="sakaw-select"
              >
                {PAO_CONFIG.map((c) => (
                  <option key={c.id} value={c.id}>
                    {c.label} — {c.months} month PAO
                  </option>
                ))}
              </select>
              <ChevronDown size={16} className="sakaw-select-chevron" />
            </div>
          </div>
          <div>
            <label className="sakaw-label">Date opened</label>
            <div className="relative mt-2">
              <input
                type="date"
                value={dateOpened}
                max={new Date().toISOString().split("T")[0]}
                onChange={(e) => setDateOpened(e.target.value)}
                className="sakaw-input"
              />
              <CalendarDays size={16} className="sakaw-select-chevron" />
            </div>
          </div>
        </div>
      </div>

      {!result && (
        <div className="sakaw-glass rounded-3xl p-8 text-center sakaw-fade-in">
          <p className="sakaw-body-soft">Choose a date opened above to see your product's shelf-life status.</p>
        </div>
      )}

      {result && (
        <div className="sakaw-fade-in">
          <div className="sakaw-glass-strong rounded-3xl p-6 md:p-10 mb-6 flex flex-col md:flex-row items-center gap-8">
            <div className="relative shrink-0" style={{ width: 184, height: 184 }}>
              <svg width="184" height="184" viewBox="0 0 184 184" className="sakaw-progress-ring">
                <circle cx="92" cy="92" r={radius} className="sakaw-ring-track" fill="none" strokeWidth="14" />
                <circle
                  cx="92"
                  cy="92"
                  r={radius}
                  fill="none"
                  strokeWidth="14"
                  strokeLinecap="round"
                  strokeDasharray={circumference}
                  strokeDashoffset={dashoffset}
                  className={result.isExpired ? "sakaw-ring-progress-expired" : "sakaw-ring-progress-safe"}
                  transform="rotate(-90 92 92)"
                />
              </svg>
              <div className="absolute inset-0 flex flex-col items-center justify-center text-center px-4">
                {result.isExpired ? (
                  <>
                    <AlertTriangle size={26} className="sakaw-icon-expired mb-1" />
                    <span className="sakaw-ring-text-sm">Expired</span>
                  </>
                ) : (
                  <>
                    <span className="sakaw-ring-text-lg">{result.remainingDays}</span>
                    <span className="sakaw-ring-text-sm">days remaining</span>
                  </>
                )}
              </div>
            </div>

            <div className="flex-1">
              <div className={`sakaw-status-badge ${result.isExpired ? "sakaw-status-expired" : "sakaw-status-safe"}`}>
                {result.isExpired ? <AlertTriangle size={15} /> : <ShieldCheck size={15} />}
                {result.isExpired ? "Expired! Discard Product" : "Safe to Use"}
              </div>

              <dl className="grid grid-cols-2 gap-4 mt-5">
                <div>
                  <dt className="sakaw-dt">Category</dt>
                  <dd className="sakaw-dd">{category.label}</dd>
                </div>
                <div>
                  <dt className="sakaw-dt">PAO period</dt>
                  <dd className="sakaw-dd">{category.months} months</dd>
                </div>
                <div>
                  <dt className="sakaw-dt">Date opened</dt>
                  <dd className="sakaw-dd sakaw-mono">{formatDate(result.opened)}</dd>
                </div>
                <div>
                  <dt className="sakaw-dt">Expiration date</dt>
                  <dd className="sakaw-dd sakaw-mono">{formatDate(result.expiration)}</dd>
                </div>
              </dl>

              {!result.isExpired && (
                <p className="sakaw-body-soft mt-4">
                  {result.remainingDays} of {result.totalDays} days of safe wear remain — that's{" "}
                  {Math.round(result.percentRemaining)}% of this product's shelf life.
                </p>
              )}
              {result.isExpired && (
                <p className="sakaw-body-soft mt-4">
                  This product passed its Period After Opening on {formatDate(result.expiration)}. For your
                  skin's safety, it's time to replace it.
                </p>
              )}
            </div>
          </div>

          <AdSlot label="Advertisement" variant="inline" />
        </div>
      )}
    </div>
  );
}

/* ============================================================================
   TOOL 3 — Sakaw Skin Type & Makeup Match Quiz
   ============================================================================ */

function SkinQuiz() {
  const [step, setStep] = useState(0);
  const [answers, setAnswers] = useState([]);

  const finished = step >= QUIZ_QUESTIONS.length;

  function selectOption(type) {
    const next = [...answers, type];
    setAnswers(next);
    setStep(step + 1);
  }

  function reset() {
    setStep(0);
    setAnswers([]);
  }

  const result = useMemo(() => {
    if (!finished) return null;
    const counts = { Oily: 0, Dry: 0, Combination: 0, Sensitive: 0 };
    answers.forEach((t) => (counts[t] += 1));
    let winner = "Combination";
    let max = -1;
    ["Combination", "Sensitive", "Oily", "Dry"].forEach((t) => {
      if (counts[t] > max) {
        max = counts[t];
        winner = t;
      }
    });
    return SKIN_PROFILES[winner];
  }, [finished, answers]);

  return (
    <div className="sakaw-fade-in">
      <SectionEyebrow>Sakaw Skin Type & Makeup Match Quiz</SectionEyebrow>
      <h2 className="sakaw-h2 mt-1">Four questions to your skin profile</h2>
      <p className="sakaw-body-soft mt-2 max-w-xl mb-6">
        Answer honestly about how your skin behaves day to day. Sakaw will diagnose your skin type
        and recommend the makeup textures that will perform best on you.
      </p>

      {!finished && (
        <>
          <div className="flex items-center gap-2 mb-7">
            {QUIZ_QUESTIONS.map((q, i) => (
              <div key={q.id} className={`sakaw-quiz-dot ${i < step ? "sakaw-quiz-dot-done" : ""} ${i === step ? "sakaw-quiz-dot-active" : ""}`} />
            ))}
            <span className="sakaw-option-tag ml-2">Question {step + 1} of {QUIZ_QUESTIONS.length}</span>
          </div>

          <div className="sakaw-glass rounded-3xl p-5 md:p-8 sakaw-fade-in" key={step}>
            <h3 className="sakaw-h4 mb-5">{QUIZ_QUESTIONS[step].question}</h3>
            <div className="grid grid-cols-1 gap-3">
              {QUIZ_QUESTIONS[step].options.map((opt) => (
                <button key={opt.text} onClick={() => selectOption(opt.type)} className="sakaw-quiz-option">
                  <span>{opt.text}</span>
                  <ArrowRight size={16} className="sakaw-quiz-option-arrow" />
                </button>
              ))}
            </div>
          </div>
        </>
      )}

      {finished && result && (
        <div className="sakaw-fade-in">
          <div className="sakaw-glass-strong rounded-3xl p-6 md:p-9 mb-6">
            <div className="flex items-center justify-between flex-wrap gap-4 mb-5">
              <div>
                <p className="sakaw-eyebrow">Sakaw Skin Profile Report</p>
                <h3 className="sakaw-h2 mt-1">{result.title} Skin</h3>
              </div>
              <span className="sakaw-result-icon-wrap">
                <result.icon size={28} />
              </span>
            </div>

            <p className="sakaw-body-soft mb-6">{result.description}</p>

            <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
              <div>
                <h4 className="sakaw-h5 mb-3">Professional tips</h4>
                <ul className="space-y-2.5">
                  {result.tips.map((tip) => (
                    <li key={tip} className="sakaw-tip-item">
                      <Check size={15} className="sakaw-tip-check" />
                      <span>{tip}</span>
                    </li>
                  ))}
                </ul>
              </div>
              <div>
                <h4 className="sakaw-h5 mb-3">Recommended textures</h4>
                <div className="flex flex-wrap gap-2">
                  {result.textures.map((t) => (
                    <span key={t} className="sakaw-pill">{t}</span>
                  ))}
                </div>
              </div>
            </div>

            <button onClick={reset} className="sakaw-btn-ghost mt-7">
              <RotateCcw size={15} />
              Retake the quiz
            </button>
          </div>

          <AdSlot label="Advertisement" variant="inline" />
        </div>
      )}
    </div>
  );
}

/* ============================================================================
   Layout — Navbar / Hero / Footer
   ============================================================================ */

function Navbar({ active, setActive }) {
  return (
    <header className="sakaw-navbar sticky top-0 z-50">
      <div className="max-w-6xl mx-auto px-4 md:px-8">
        <div className="flex items-center justify-between py-4">
          <div className="flex items-center gap-3">
            <ShadeMark size={38} />
            <div className="flex flex-col leading-none">
              <span className="sakaw-logo-text">Sakaw</span>
              <span className="sakaw-logo-sub">BEAUTYTOOLS</span>
            </div>
          </div>
          <span className="sakaw-navbar-tag hidden sm:inline-flex">
            <Sparkles size={13} />
            Premium Beauty Intelligence
          </span>
        </div>
        <nav className="flex gap-2 overflow-x-auto pb-3 sakaw-scroll-hide">
          {TABS.map((tab) => {
            const Icon = tab.icon;
            const isActive = active === tab.id;
            return (
              <button
                key={tab.id}
                onClick={() => setActive(tab.id)}
                className={`sakaw-tab ${isActive ? "sakaw-tab-active" : ""}`}
              >
                <Icon size={16} />
                {tab.label}
              </button>
            );
          })}
        </nav>
      </div>
    </header>
  );
}

function Hero({ active }) {
  const copy = {
    shade: {
      title: "Precision color-matching, refined.",
      sub: "Cross-reference your shade across the world's leading foundation brands in seconds.",
    },
    pao: {
      title: "Know exactly when to let go.",
      sub: "Track the Period After Opening for every product in your routine, beautifully visualized.",
    },
    quiz: {
      title: "Understand your skin, properly.",
      sub: "Four quick questions, one professional-grade skin profile built just for you.",
    },
  }[active];

  return (
    <section className="sakaw-hero relative overflow-hidden">
      <div className="sakaw-blob sakaw-blob-1" aria-hidden="true" />
      <div className="sakaw-blob sakaw-blob-2" aria-hidden="true" />
      <div className="max-w-6xl mx-auto px-4 md:px-8 py-12 md:py-16 relative">
        <p className="sakaw-eyebrow">Sakaw BeautyTools</p>
        <h1 className="sakaw-h1 mt-2 max-w-2xl">{copy.title}</h1>
        <p className="sakaw-body-soft mt-3 max-w-xl">{copy.sub}</p>
        <div className="flex flex-wrap gap-x-8 gap-y-2 mt-6">
          <span className="sakaw-stat"><strong>5</strong> global brands</span>
          <span className="sakaw-stat"><strong>75+</strong> shades mapped</span>
          <span className="sakaw-stat"><strong>3</strong> Sakaw tools</span>
        </div>
      </div>
    </section>
  );
}

function Footer() {
  return (
    <footer className="sakaw-footer mt-16">
      <div className="max-w-6xl mx-auto px-4 md:px-8 py-10">
        <div className="flex flex-col md:flex-row items-start md:items-center justify-between gap-6 pb-8 sakaw-footer-divider">
          <div className="flex items-center gap-3">
            <ShadeMark size={32} />
            <div className="flex flex-col leading-none">
              <span className="sakaw-logo-text sakaw-logo-text-light">Sakaw</span>
              <span className="sakaw-logo-sub sakaw-logo-sub-light">BEAUTYTOOLS</span>
            </div>
          </div>
          <p className="sakaw-footer-tagline">Beauty tools, calibrated with precision.</p>
        </div>
        <div className="flex flex-col md:flex-row justify-between gap-4 pt-6">
          <p className="sakaw-footer-credit">© 2026 Sakaw BeautyTools. Crafted by Sakaw.</p>
          <p className="sakaw-footer-disclaimer max-w-xl">
            Shade and product data shown are for demonstration purposes only. Always confirm a match
            in natural light before purchasing.
          </p>
        </div>
      </div>
    </footer>
  );
}

/* ============================================================================
   App
   ============================================================================ */

export default function App() {
  const [active, setActive] = useState("shade");

  useEffect(() => {
    document.title = "Sakaw BeautyTools";
  }, []);

  return (
    <div className="sakaw-app min-h-screen flex flex-col">
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,600;0,700;1,500&family=Manrope:wght@400;500;600;700;800&family=JetBrains+Mono:wght@500;600&display=swap');

        .sakaw-app {
          --cream: #FBF5EF;
          --cream-deep: #F3E7DC;
          --blush: #F3D6DE;
          --blush-deep: #E8B9C6;
          --rosegold: #B76E79;
          --rosegold-deep: #9C5C66;
          --charcoal: #2B2521;
          --charcoal-soft: #6B5F58;
          --green: #4C8B6E;
          --red: #BE5A4E;
          background: linear-gradient(180deg, var(--cream) 0%, var(--cream-deep) 100%);
          color: var(--charcoal);
          font-family: 'Manrope', sans-serif;
        }

        .sakaw-app * { box-sizing: border-box; }

        /* Typography */
        .sakaw-h1 { font-family:'Cormorant Garamond',serif; font-weight:600; font-size:2.1rem; line-height:1.1; color:var(--charcoal); }
        @media (min-width:768px){ .sakaw-h1{ font-size:3rem; } }
        .sakaw-h2 { font-family:'Cormorant Garamond',serif; font-weight:600; font-size:1.65rem; line-height:1.2; color:var(--charcoal); }
        @media (min-width:768px){ .sakaw-h2{ font-size:2.1rem; } }
        .sakaw-h4 { font-family:'Manrope',sans-serif; font-weight:700; font-size:1.05rem; color:var(--charcoal); }
        .sakaw-h5 { font-family:'Manrope',sans-serif; font-weight:700; font-size:0.92rem; letter-spacing:.02em; color:var(--charcoal); text-transform:uppercase; }
        .sakaw-body-soft { font-family:'Manrope',sans-serif; font-size:0.95rem; color:var(--charcoal-soft); line-height:1.6; }
        .sakaw-eyebrow { font-family:'Manrope',sans-serif; font-weight:700; font-size:0.72rem; letter-spacing:.18em; text-transform:uppercase; color:var(--rosegold-deep); }
        .sakaw-strong { color:var(--charcoal); font-weight:700; }
        .sakaw-mono { font-family:'JetBrains Mono',monospace; }

        /* Logo */
        .sakaw-logo-text { font-family:'Cormorant Garamond',serif; font-weight:600; font-size:1.7rem; letter-spacing:.01em; color:var(--charcoal); }
        .sakaw-logo-sub { font-family:'Manrope',sans-serif; font-weight:800; font-size:0.62rem; letter-spacing:.28em; color:var(--rosegold); }
        .sakaw-logo-text-light { color: #FBF5EF; }
        .sakaw-logo-sub-light { color: var(--blush-deep); }

        /* Navbar */
        .sakaw-navbar { background: rgba(251,245,239,0.85); backdrop-filter: blur(14px); border-bottom: 1px solid rgba(183,110,121,0.16); }
        .sakaw-navbar-tag { align-items:center; gap:6px; font-size:0.72rem; font-weight:600; letter-spacing:.04em; color:var(--rosegold-deep); background: rgba(243,214,222,0.5); border:1px solid rgba(183,110,121,0.25); border-radius:999px; padding:6px 14px; }
        .sakaw-tab { display:flex; align-items:center; gap:7px; white-space:nowrap; font-weight:600; font-size:0.85rem; color:var(--charcoal-soft); background:rgba(255,255,255,0.5); border:1px solid rgba(183,110,121,0.18); border-radius:999px; padding:9px 18px; transition: all .25s ease; }
        .sakaw-tab:hover { background:rgba(255,255,255,0.85); color:var(--charcoal); transform: translateY(-1px); }
        .sakaw-tab-active { background: linear-gradient(135deg, var(--rosegold), #C98F8A); color:#fff; border-color: transparent; box-shadow: 0 8px 20px rgba(183,110,121,0.32); }
        .sakaw-tab-active:hover { transform:none; color:#fff; background: linear-gradient(135deg, var(--rosegold), #C98F8A); }
        .sakaw-scroll-hide::-webkit-scrollbar { display:none; }
        .sakaw-scroll-hide { scrollbar-width:none; }

        /* Hero */
        .sakaw-hero { background: linear-gradient(135deg, rgba(243,214,222,0.55), rgba(251,245,239,0)); }
        .sakaw-blob { position:absolute; border-radius:50%; filter: blur(50px); opacity:0.55; animation: sakawFloat 14s ease-in-out infinite; }
        .sakaw-blob-1 { width:280px; height:280px; background: var(--blush); top:-90px; right:-60px; }
        .sakaw-blob-2 { width:200px; height:200px; background: var(--rosegold); opacity:0.25; bottom:-80px; left:10%; animation-delay: -7s; }
        .sakaw-stat { font-size:0.85rem; color: var(--charcoal-soft); }
        .sakaw-stat strong { font-family:'JetBrains Mono',monospace; color:var(--rosegold-deep); font-weight:600; }

        /* Glass cards */
        .sakaw-glass { background: rgba(255,255,255,0.55); backdrop-filter: blur(16px); border:1px solid rgba(255,255,255,0.7); box-shadow: 0 8px 32px rgba(183,110,121,0.10); }
        .sakaw-glass-strong { background: rgba(255,255,255,0.72); backdrop-filter: blur(20px); border:1px solid rgba(255,255,255,0.85); box-shadow: 0 14px 40px rgba(183,110,121,0.16); }

        /* Buttons */
        .sakaw-btn-ghost { display:inline-flex; align-items:center; gap:7px; font-weight:600; font-size:0.85rem; color:var(--rosegold-deep); background:rgba(255,255,255,0.6); border:1px solid rgba(183,110,121,0.3); border-radius:999px; padding:9px 18px; transition: all .25s ease; cursor:pointer; }
        .sakaw-btn-ghost:hover { background:#fff; transform: translateY(-1px); box-shadow: 0 6px 16px rgba(183,110,121,0.18); }

        /* Step indicator (Shade Finder) */
        .sakaw-step-dot { width:26px; height:26px; border-radius:50%; display:flex; align-items:center; justify-content:center; font-size:0.75rem; font-weight:700; background:rgba(255,255,255,0.6); border:1px solid rgba(183,110,121,0.25); color: var(--charcoal-soft); }
        .sakaw-step-active { background: linear-gradient(135deg, var(--rosegold), #C98F8A); color:#fff; border-color:transparent; }
        .sakaw-step-done { background: var(--blush-deep); color: var(--rosegold-deep); border-color:transparent; }
        .sakaw-step-label { font-size:0.82rem; font-weight:600; color: var(--charcoal-soft); }
        .sakaw-step-label-active { color: var(--charcoal); }
        .sakaw-step-chevron { color: rgba(183,110,121,0.4); }

        /* Option cards (brand/product selectors) */
        .sakaw-option-card { display:flex; flex-direction:column; align-items:center; gap:8px; padding:16px 10px; border-radius:18px; background:rgba(255,255,255,0.55); border:1px solid rgba(183,110,121,0.18); transition: all .25s ease; cursor:pointer; text-align:center; }
        .sakaw-option-card:hover { transform: translateY(-3px); background:rgba(255,255,255,0.9); box-shadow: 0 10px 24px rgba(183,110,121,0.16); }
        .sakaw-option-card-active { background: linear-gradient(160deg, rgba(243,214,222,0.7), rgba(255,255,255,0.9)); border-color: var(--rosegold); box-shadow: 0 10px 24px rgba(183,110,121,0.22); }
        .sakaw-option-card-wide { flex-direction:row; align-items:flex-start; justify-content:space-between; text-align:left; gap:4px; }
        .sakaw-monogram { width:38px; height:38px; border-radius:50%; display:flex; align-items:center; justify-content:center; font-family:'JetBrains Mono',monospace; font-weight:600; font-size:0.7rem; color:#fff; background: linear-gradient(135deg, var(--rosegold), var(--rosegold-deep)); }
        .sakaw-monogram-sm { width:30px; height:30px; font-size:0.62rem; }
        .sakaw-option-label { font-size:0.82rem; font-weight:600; color: var(--charcoal); }
        .sakaw-option-label-lg { font-size:0.9rem; font-weight:700; color: var(--charcoal); }
        .sakaw-option-tag { font-size:0.74rem; color: var(--charcoal-soft); }

        /* Shade cards */
        .sakaw-shade-card { display:flex; flex-direction:column; align-items:center; gap:6px; padding:14px 8px; border-radius:16px; background:rgba(255,255,255,0.55); border:1px solid rgba(183,110,121,0.18); transition: all .25s ease; cursor:pointer; }
        .sakaw-shade-card:hover { transform: translateY(-3px); background:rgba(255,255,255,0.9); }
        .sakaw-shade-card-active { border-color: var(--rosegold); background: rgba(255,255,255,0.95); box-shadow: 0 10px 22px rgba(183,110,121,0.2); }
        .sakaw-shade-dot { width:30px; height:30px; border-radius:50%; border:2px solid rgba(255,255,255,0.9); box-shadow: 0 2px 8px rgba(0,0,0,0.12); }
        .sakaw-shade-dot-lg { width:54px; height:54px; border-radius:50%; border:3px solid rgba(255,255,255,0.95); box-shadow: 0 4px 14px rgba(0,0,0,0.14); }
        .sakaw-shade-code { font-family:'JetBrains Mono',monospace; font-size:0.74rem; font-weight:600; color: var(--charcoal); }
        .sakaw-shade-meta { font-size:0.68rem; color: var(--charcoal-soft); }

        /* Result cards */
        .sakaw-result-card { background:rgba(255,255,255,0.6); border:1px solid rgba(183,110,121,0.18); border-radius:20px; padding:18px; transition: all .25s ease; }
        .sakaw-result-card:hover { transform: translateY(-4px); box-shadow: 0 14px 30px rgba(183,110,121,0.18); background:rgba(255,255,255,0.85); }
        .sakaw-result-brand { font-family:'Cormorant Garamond',serif; font-weight:600; font-size:1.1rem; color: var(--charcoal); }
        .sakaw-result-product { font-size:0.82rem; color: var(--charcoal-soft); margin-top:1px; }
        .sakaw-result-shade { font-family:'JetBrains Mono',monospace; font-size:0.8rem; color: var(--rosegold-deep); margin-top:6px; }
        .sakaw-match-badge { display:inline-flex; align-items:center; gap:5px; font-size:0.65rem; font-weight:700; letter-spacing:.02em; color: var(--rosegold-deep); background: rgba(243,214,222,0.55); border:1px solid rgba(183,110,121,0.25); border-radius:999px; padding:5px 10px; }

        /* Form controls */
        .sakaw-label { font-size:0.78rem; font-weight:700; letter-spacing:.05em; text-transform:uppercase; color: var(--charcoal-soft); }
        .sakaw-select, .sakaw-input { width:100%; appearance:none; background: rgba(255,255,255,0.7); border:1px solid rgba(183,110,121,0.3); border-radius:14px; padding:12px 40px 12px 16px; font-family:'Manrope',sans-serif; font-weight:600; font-size:0.9rem; color: var(--charcoal); transition: all .2s ease; }
        .sakaw-select:focus, .sakaw-input:focus { outline:none; border-color: var(--rosegold); box-shadow: 0 0 0 3px rgba(183,110,121,0.18); }
        .sakaw-select-chevron { position:absolute; right:14px; top:50%; transform:translateY(-50%); color: var(--rosegold-deep); pointer-events:none; }

        /* PAO ring + status */
        .sakaw-ring-track { stroke: rgba(183,110,121,0.15); }
        .sakaw-ring-progress-safe { stroke: var(--green); transition: stroke-dashoffset 1s ease-out; }
        .sakaw-ring-progress-expired { stroke: var(--red); transition: stroke-dashoffset 1s ease-out; }
        .sakaw-ring-text-lg { font-family:'JetBrains Mono',monospace; font-size:2rem; font-weight:600; color: var(--charcoal); line-height:1; }
        .sakaw-ring-text-sm { font-size:0.78rem; color: var(--charcoal-soft); margin-top:4px; }
        .sakaw-icon-expired { color: var(--red); }
        .sakaw-status-badge { display:inline-flex; align-items:center; gap:7px; font-weight:700; font-size:0.85rem; border-radius:999px; padding:9px 18px; }
        .sakaw-status-safe { background: rgba(76,139,110,0.12); color: var(--green); border:1px solid rgba(76,139,110,0.3); }
        .sakaw-status-expired { background: rgba(190,90,78,0.12); color: var(--red); border:1px solid rgba(190,90,78,0.3); }
        .sakaw-dt { font-size:0.68rem; letter-spacing:.06em; text-transform:uppercase; color: var(--charcoal-soft); }
        .sakaw-dd { font-size:0.92rem; font-weight:700; color: var(--charcoal); margin-top:2px; }

        /* Quiz */
        .sakaw-quiz-dot { width:34px; height:6px; border-radius:999px; background: rgba(183,110,121,0.18); transition: all .3s ease; }
        .sakaw-quiz-dot-done { background: var(--blush-deep); }
        .sakaw-quiz-dot-active { background: linear-gradient(90deg, var(--rosegold), #C98F8A); }
        .sakaw-quiz-option { display:flex; align-items:center; justify-content:space-between; gap:10px; text-align:left; background: rgba(255,255,255,0.55); border:1px solid rgba(183,110,121,0.2); border-radius:16px; padding:15px 18px; font-weight:600; font-size:0.9rem; color: var(--charcoal); transition: all .22s ease; cursor:pointer; }
        .sakaw-quiz-option:hover { background: rgba(255,255,255,0.92); border-color: var(--rosegold); transform: translateX(3px); }
        .sakaw-quiz-option-arrow { color: rgba(183,110,121,0.45); flex-shrink:0; }
        .sakaw-quiz-option:hover .sakaw-quiz-option-arrow { color: var(--rosegold); }
        .sakaw-result-icon-wrap { width:54px; height:54px; border-radius:50%; display:flex; align-items:center; justify-content:center; background: linear-gradient(135deg, var(--blush), var(--blush-deep)); color: var(--rosegold-deep); }
        .sakaw-tip-item { display:flex; align-items:flex-start; gap:8px; font-size:0.88rem; color: var(--charcoal-soft); line-height:1.5; }
        .sakaw-tip-check { color: var(--green); margin-top:3px; flex-shrink:0; }
        .sakaw-pill { font-size:0.78rem; font-weight:600; color: var(--rosegold-deep); background: rgba(243,214,222,0.5); border:1px solid rgba(183,110,121,0.25); border-radius:999px; padding:6px 14px; }

        /* Ad slots */
        .sakaw-ad-slot { background: rgba(255,255,255,0.4); border: 1px dashed rgba(183,110,121,0.4); }
        .sakaw-ad-label { font-size:0.72rem; font-weight:700; letter-spacing:.12em; text-transform:uppercase; color: var(--rosegold-deep); }
        .sakaw-ad-sub { font-size:0.7rem; color: var(--charcoal-soft); }

        /* Footer */
        .sakaw-footer { background: var(--charcoal); color: #EFE3DC; }
        .sakaw-footer-divider { border-bottom: 1px solid rgba(255,255,255,0.12); }
        .sakaw-footer-tagline { font-family:'Cormorant Garamond',serif; font-style:italic; font-size:1rem; color: var(--blush-deep); }
        .sakaw-footer-credit { font-size:0.82rem; color: rgba(239,227,220,0.75); }
        .sakaw-footer-disclaimer { font-size:0.76rem; color: rgba(239,227,220,0.5); line-height:1.5; }

        /* Animations */
        @keyframes sakawFadeIn { from { opacity:0; transform: translateY(10px); } to { opacity:1; transform: translateY(0); } }
        .sakaw-fade-in { animation: sakawFadeIn .5s ease-out both; }
        @keyframes sakawFloat { 0%,100% { transform: translateY(0) scale(1); } 50% { transform: translateY(-18px) scale(1.05); } }

        @media (prefers-reduced-motion: reduce) {
          .sakaw-fade-in, .sakaw-blob { animation: none !important; }
          .sakaw-option-card, .sakaw-tab, .sakaw-result-card, .sakaw-quiz-option, .sakaw-shade-card, .sakaw-btn-ghost { transition: none !important; }
        }

        .sakaw-app button:focus-visible, .sakaw-app select:focus-visible, .sakaw-app input:focus-visible {
          outline: 2px solid var(--rosegold);
          outline-offset: 2px;
        }
      `}</style>

      <Navbar active={active} setActive={setActive} />
      <Hero active={active} />

      <main className="flex-1 max-w-6xl mx-auto px-4 md:px-8 w-full">
        <div className="mb-8">
          <AdSlot label="Top Banner Advertisement" variant="banner" />
        </div>

        <div className="grid grid-cols-1 lg:grid-cols-4 gap-8 pb-12">
          <div className="lg:col-span-3" key={active}>
            {active === "shade" && <ShadeFinder />}
            {active === "pao" && <PaoCalculator />}
            {active === "quiz" && <SkinQuiz />}
          </div>

          <aside className="lg:col-span-1">
            <div className="hidden lg:block sticky top-32">
              <AdSlot label="Sidebar Advertisement" variant="sidebar" />
            </div>
            <div className="lg:hidden mt-2">
              <AdSlot label="Advertisement" variant="banner" />
            </div>
          </aside>
        </div>
      </main>

      <Footer />
    </div>
  );
}
