import React, { useState } from 'react';

// A 2026-style "Mission Control" Landing Component
const MindshareHero = () => {
  const [activeMissions, setActiveMissions] = useState(1284);

  return (
    <div className="min-h-screen bg-black text-emerald-400 font-mono p-8 selection:bg-emerald-900">
      {/* Top Navigation Bar */}
      <nav className="flex justify-between border-b border-emerald-900/50 pb-4 mb-12">
        <div className="text-2xl font-bold tracking-tighter">MINDSHARE_OS v1.0</div>
        <div className="space-x-8 text-sm opacity-70">
          <span>LIVE_MISSIONS: {activeMissions}</span>
          <span>$MIND: $2.42 (+12%)</span>
          <button className="border border-emerald-400 px-4 py-1 hover:bg-emerald-400 hover:text-black transition-all">
            CONNECT_SYNAPSE
          </button>
        </div>
      </nav>

      {/* Main Command Console */}
      <main className="grid grid-cols-12 gap-8">
        {/* Left: Swarm Status */}
        <div className="col-span-3 border border-emerald-900/30 p-4 bg-emerald-950/10 backdrop-blur-md">
          <h2 className="text-xs mb-4 opacity-50 underline">ACTIVE_SWARMS</h2>
          <ul className="space-y-4 text-xs">
            <li className="flex justify-between"><span>SWARM_ALFA (Marketing)</span> <span className="text-white">RUNNING</span></li>
            <li className="flex justify-between"><span>SWARM_BETA (Code_Gen)</span> <span className="text-yellow-500">OPTIMIZING</span></li>
            <li className="animate-pulse"><span>> ANALYZING_GLOBAL_INTENT...</span></li>
          </ul>
        </div>

        {/* Center: The Big Idea */}
        <div className="col-span-6 text-center py-20">
          <h1 className="text-6xl font-black mb-6 tracking-tighter text-white">
            DON'T BET ON THE FUTURE. <br/>
            <span className="text-emerald-400">PROGRAM IT.</span>
          </h1>
          <p className="max-w-md mx-auto text-sm opacity-80 mb-10">
            The world's first Generative Action Market. Deploy AI swarms to achieve collective goals and earn $MIND.
          </p>
          <div className="flex justify-center gap-4">
            <button className="bg-emerald-400 text-black font-bold px-8 py-4 text-lg hover:scale-105 transition-transform">
              CREATE_MISSION
            </button>
            <button className="border border-emerald-400 px-8 py-4 text-lg hover:bg-emerald-400/10">
              JOIN_THE_SWARM
            </button>
          </div>
        </div>

        {/* Right: Real-time Oracle Feed */}
        <div className="col-span-3 border border-emerald-900/30 p-4 bg-emerald-950/10 overflow-hidden">
          <h2 className="text-xs mb-4 opacity-50 underline">GLOBAL_ORACLE_FEED</h2>
          <div className="text-[10px] space-y-2 opacity-60">
            <p>[14:02:11] Mission #882: "Clean_Pacific" milestone reached.</p>
            <p>[14:02:15] $MIND payout triggered for 4,200 nodes.</p>
            <p>[14:02:22] New Mission: "Lobby_For_AI_Rights" launched by @UserX.</p>
          </div>
        </div>
      </main>

      {/* Footer / Data Strip */}
      <footer className="fixed bottom-0 left-0 w-full p-4 border-t border-emerald-900/50 bg-black/80 backdrop-blur-xl flex gap-12 overflow-hidden whitespace-nowrap italic text-xs opacity-40">
        <span>MISSION_SUCCESS_RATE: 94.2%</span>
        <span>TOTAL_VALUE_LOCKED: $1.2B</span>
        <span>AGENT_UPTIME: 99.9999%</span>
        <span>ACTIVE_NODES: 8.4M</span>
      </footer>
    </div>
  );
};

export default MindshareHero;
