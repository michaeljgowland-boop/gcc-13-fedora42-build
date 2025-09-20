# Extract the tarball in root or desired prefix
sudo tar -xzf gcc-13.3-fedora42.tar.gz -C /usr/local/

# Add the new GCC to your PATH and LD_LIBRARY_PATH
export PATH=/usr/local/gcc-13.3/bin:$PATH
export LD_LIBRARY_PATH=/usr/local/gcc-13.3/lib64:/usr/local/gcc-13.3/lib:$LD_LIBRARY_PATH

# Verify
gcc-13 --version
g++-13 --version
