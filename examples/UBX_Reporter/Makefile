# Makefile for building, uploading, and maintaining Arduino UBX_Reader example
# for those who want to avoid the Arduino IDE.
#
# Copyright (C) 2015 Simon D. Levy
#
# This code is free software: you can redistribute it and/or modify
# it under the terms of the GNU Lesser General Public License as 
# published by the Free Software Foundation, either version 3 of the 
# License, or (at your option) any later version.
# 
# This code is distributed in the hope that it will be useful,     
# but WITHOUT ANY WARRANTY without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# 
# You should have received a copy of the GNU Lesser General Public License 
# along with this code.  If not, see <http://www.gnu.org/licenses/>.

PORT = ACM0

all: build

edit:
	vim UBX_Reporter.ino

build: UBX_Reporter.ino
	arduino --verify UBX_Reporter.ino

upload: UBX_Reporter.ino
	arduino --upload UBX_Reporter.ino

probe:
	ls /dev/ttyA*

mini:
	miniterm.py /dev/tty$(PORT) 9600 --exit-char=27
