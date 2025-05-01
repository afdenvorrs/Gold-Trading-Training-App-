import React from "react";
import Link from "next/link"; // If using Next.js
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Trophy, LineChart, BookOpen, Gamepad2 } from "lucide-react";

export default function GoldTradeMastery() {
  return (
    <main className="p-6 space-y-6 max-w-4xl mx-auto">
      <header>
        <h1 className="text-3xl font-bold text-center">GoldTrade Mastery</h1>
      </header>

      <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
        {/* Learning Modules */}
        <section aria-labelledby="learning-modules">
          <Card className="hover:shadow-lg transition-shadow duration-300">
            <CardContent className="p-4">
              <div className="flex items-center space-x-3">
                <BookOpen className="w-6 h-6" />
                <h2 id="learning-modules" className="text-xl font-semibold">
                  Interactive Learning Modules
                </h2>
              </div>
              <p className="mt-2 text-sm text-muted-foreground">
                Unlock lessons on technical indicators, candlestick patterns, and risk management from beginner to advanced.
              </p>
            </CardContent>
          </Card>
        </section>

        {/* Simulated Trading */}
        <section aria-labelledby="simulated-trading">
          <Card className="hover:shadow-lg transition-shadow duration-300">
            <CardContent className="p-4">
              <div className="flex items-center space-x-3">
                <LineChart className="w-6 h-6" />
                <h2 id="simulated-trading" className="text-xl font-semibold">
                  Simulated Trading Arena
                </h2>
              </div>
              <p className="mt-2 text-sm text-muted-foreground">
                Practice trading gold with virtual funds using real or simulated market data.
              </p>
            </CardContent>
          </Card>
        </section>

        {/* Gamified Quests */}
        <section aria-labelledby="gamified-quests">
          <Card className="hover:shadow-lg transition-shadow duration-300">
            <CardContent className="p-4">
              <div className="flex items-center space-x-3">
                <Gamepad2 className="w-6 h-6" />
                <h2 id="gamified-quests" className="text-xl font-semibold">
                  Gamified Quests
                </h2>
              </div>
              <p className="mt-2 text-sm text-muted-foreground">
                Complete missions like “Spot the Trend” or “MACD Divergence Hunt” and earn badges.
              </p>
            </CardContent>
          </Card>
        </section>

        {/* Leaderboards */}
        <section aria-labelledby="leaderboard">
          <Card className="hover:shadow-lg transition-shadow duration-300">
            <CardContent className="p-4">
              <div className="flex items-center space-x-3">
                <Trophy className="w-6 h-6" />
                <h2 id="leaderboard" className="text-xl font-semibold">
                  Leaderboard & Challenges
                </h2>
              </div>
              <p className="mt-2 text-sm text-muted-foreground">
                Rank up with smart trades and challenge other users in weekly gold trading contests.
              </p>
            </CardContent>
          </Card>
        </section>
      </div>

      <div className="text-center">
        <Button asChild className="text-lg px-6 py-3 rounded-2xl shadow-md">
          <Link href="/learning">Start Learning</Link>
        </Button>
      </div>
    </main>
  );
}
