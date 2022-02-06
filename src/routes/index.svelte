<script>
    import supabase from '$lib/db';

    
    async function logout() {
   	 const { error } = await supabase.auth.signOut();

   	 if (error) alert(error.message); // alert if error
    }

</script>
let timetable =   { Monday: [
    {
      name: "PH", //Perhimpunan (Morning Assembly)
      period: 1,
      style: "",
    },
    {
      name: "PM", // Pendidikan Moral (Moral Studies)
      period: 2,
      style: "",
    },
    {
      name: "BI", // Bahasa Inggeris (English Subject)
      period: 3,
      style: "",
    }
    {
      name: "BM", // Bahasa Melayu (Bahasa Subject)
      period: 4,
      style: "",
    }
    {
      name: "BC", // Bahasa Chinese (Chinese Subject)
      period: 5,
      style: "",
    }
    {
      name: "MAT", // Mathematics (Math Subject)
      period: 6,
      style: "",
    }
    {
      name: "SNS", // Science (Science Subject)
      period: 7,
      style: "",
    }
    {
      name: "GEO", // Geography (Geography Subject)
      period: 8,
      style: "",
    }
    {
      name: "SEJ", // Sejarah (Sejarah Subject)
      period: 9,
      style: "",
    }
    {
      name: "BC", // Bahasa Chinese (Chinese Subject)
      period: 10,
      style: "",
    }
]},
 Tuesday: [{
    name: "PH", //Perhimpunan (Morning Assembly)
    period: 1,
    style: "",
  },
  {
    name: "PM", // Pendidikan Moral (Moral Studies)
    period: 2,
    style: "",
  },
  {
    name: "BI", // Bahasa Inggeris (English Subject)
    period: 3,
    style: "",
  }
  {
    name: "BM", // Bahasa Melayu (Bahasa Subject)
    period: 4,
    style: "",
  }
  {
    name: "BC", // Bahasa Chinese (Chinese Subject)
    period: 5,
    style: "",
  }
  {
    name: "MAT", 
    period: 6,
    style: "",
  }
  {
    name: "SNS", 
    period: 7,
    style: "",
  }
  {
    name: "GEO", 
    period: 8,
    style: "",
  }
  {
    name: "SEJ", 
    period: 9,
    style: "",
  }
  {
    name: "BC", 
    period: 10,
    style: "",
  }],
 Wednesday: [],
 Thursday: [],
 Friday: [],
};


<table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">First</th>
      <th scope="col">Last</th>
      <th scope="col">Handle</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Mark</td>
      <td>Otto</td>
      <td>@mdo</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jacob</td>
      <td>Thornton</td>
      <td>@fat</td>
    </tr>
    <tr>
      <th scope="row">3</th>
      <td colspan="2">Larry the Bird</td>
      <td>@twitter</td>
    </tr>
  </tbody>
</table>


<!-- Sign Out -->
<section class="container px-4 py-3 text-center">
    <button class="btn btn-secondary" on:click={logout}>Logout</button>
</section>	

