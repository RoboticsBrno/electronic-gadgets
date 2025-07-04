.PHONY: all

all: build/fab build/usbPad-panel.kicad_pcb

build:
	mkdir -p build

build/usbPad-panel.kicad_pcb: hardware/usbPad.kicad_pcb build
	kikit panelize \
		--layout 'grid; rows: 6; cols: 6; space: 2mm' \
		--tabs 'fixed; width: 8mm; vcount: 1; hcount: 0' \
		--cuts 'vcuts' \
		--framing 'frame; width: 5mm; space: 2mm;' \
		--post 'millradius: 1mm' \
		$< $@

build/fab: build/usbPad-panel.kicad_pcb
	kikit fab jlcpcb $< $@

clean:
	rm -rf build