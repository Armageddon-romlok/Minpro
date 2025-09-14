# Sistem Pendataan Member Gym

members = []

while True:
    print("\n=== Sistem Pendataan Member Gym ===") 
    print("1.Tambah Member")
    print("2.Lihat Data Member")
    print("3.Keluar")

    pilihan = input("Pilih menu (1/2/3): ")
    
    if pilihan == "1":
        print("\n=== Tambah Member Baru ===")
        nama = input("Masukkan Nama Member : ")
        umur = input("Masukkan Umur Member : ")
        paket = input("Masukkan Paket Gym (Bulanan/Tahunan): ")
        
        member = (nama, umur, paket)
        members.append(member)
        
        print("Member berhasil ditambahkan")
    
    elif pilihan == "2":
        print("\n===Daftar Member Gym===")
        if len(members) == 0:
            print("Belum ada data member.")
        else:
            for i, member in enumerate(members, start=1):
                print(f"{i}. Nama: {member[0]}, Umur: {member[1]}, Paket: {member[2]}")
    
    elif pilihan == "3":
        print("Terima kasih, program selesai.")
        break
    else:
        print("Pilihan tidak valid, coba lagi.")
