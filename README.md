class alquiler:
  def __init__(self, alquiler, metros_cuadrados):
    self.alquiler = alquiler
    self.metros_cuadrados = metros_cuadrados

class semestral (alquiler):
  def pago(self):
    return (self.alquiler * self.metros_cuadrados) * 6

class anual (alquiler):
  def pago(self):
    return (self.alquiler * self.metros_cuadrados) * 12

semestral = semestral (25,40)
anual = anual (30,40)

print("Pago semestral: ", semestral.pago())
print("Pago anual:", anual.pago())
