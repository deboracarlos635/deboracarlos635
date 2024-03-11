- 👋 Hi, I’m @deboracarlos635
- 👀 I’m interested in programming
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on projects
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

class Liquid:
    def _init_(self, name, density):
        self.name = name
        self.density = density

class Container:
    def _init_(self, height):
        self.liquids = []
        self.height = height

    def add_liquid(self, liquid):
        self.liquids.append(liquid)

    def calculate_pressure(self, gravity=9.81):
        total_pressure = 0
        for liquid in self.liquids:
            liquid_pressure = liquid.density * gravity * self.height
            total_pressure += liquid_pressure
        return total_pressure
