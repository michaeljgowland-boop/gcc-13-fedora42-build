# Extract the tarball in root or desired prefix
sudo tar -xzf gcc-13.3-fedora42.tar.gz -C /usr/local/

# Add the new GCC to your PATH and LD_LIBRARY_PATH
export PATH=/usr/local/gcc-13.3/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/gcc-13.3/lib64:/usr/local/gcc-13.3/lib:$LD_LIBRARY_PATH

# Verify
gcc-13 --version
g++-13 --version

## License

This software is licensed under the GNU General Public License version 3 (GPLv3).

You can freely use, modify, and redistribute this software under these terms.

The full license text is included in the `LICENSE` file in this repository.

For details, visit: https://www.gnu.org/licenses/gpl-3.0.html


Disclaimer - I offer no gurantees with this, obviusly I did not write it, I built it from source because I needed it and it was not availbe via DNF and I am sharing it to save anyone else who needs it the trouble of building it.

