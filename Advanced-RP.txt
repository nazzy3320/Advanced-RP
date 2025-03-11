import React from "react";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";

export default function AdvancedRP() {
  return (
    <div className="min-h-screen bg-gray-900 text-white flex flex-col items-center p-6">
      <header className="text-4xl font-bold my-6">Advanced RP</header>
      <Card className="w-full max-w-3xl p-4 bg-gray-800 shadow-lg rounded-2xl">
        <CardContent>
          <h2 className="text-2xl font-semibold mb-4">Регистрация</h2>
          <div className="space-y-4">
            <Input placeholder="Имя персонажа" className="bg-gray-700 text-white" />
            <Input placeholder="Email" type="email" className="bg-gray-700 text-white" />
            <Input placeholder="Пароль" type="password" className="bg-gray-700 text-white" />
            <Textarea placeholder="Краткое описание персонажа" className="bg-gray-700 text-white" />
            <Button className="w-full bg-blue-600 hover:bg-blue-700">Зарегистрироваться</Button>
          </div>
        </CardContent>
      </Card>
      
      <Card className="w-full max-w-3xl mt-6 p-4 bg-gray-800 shadow-lg rounded-2xl">
        <CardContent>
          <h2 className="text-2xl font-semibold mb-4">Правила сервера</h2>
          <ul className="list-disc pl-5 space-y-2 text-gray-300">
            <li>Уважайте других игроков.</li>
            <li>Запрещены читы и баги.</li>
            <li>Ролевой процесс должен быть реалистичным.</li>
            <li>Администрация имеет право принимать окончательные решения.</li>
          </ul>
        </CardContent>
      </Card>
    </div>
  );
}

// Добавьте этот файл в ваш репозиторий GitHub и настройте проект с помощью Vite или Next.js.
